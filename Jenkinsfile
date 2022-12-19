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
            envSettings
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
