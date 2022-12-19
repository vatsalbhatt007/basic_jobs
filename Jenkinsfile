@Library('basic-library') _
def pipelineSettings = null

pipeline {
    agent any
    stages {
        stage('Demo') {
            steps {
                echo 'Hello, world'
                helloWorld 'Vatsal'
                }
        }
        stage ('env') {
        steps{
            envSettings 'env'
            }
        }
        stage ('oc') {
            steps {
                script {
                    Ops.oc(pipelineSettings,'login')
                }
            }            
        }
    }
    post
    {
        always {
            cleanWs()
        }
    }
}
