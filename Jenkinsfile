@Library('basic-library') _

pipeline {
    agent any
    stages {
        stage('Demo') {
            steps {
                echo 'Hello, world'
                helloWorld 'Vatsal'
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
