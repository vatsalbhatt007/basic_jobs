@Library('basic-library') _

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
                Ops('','login')
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
