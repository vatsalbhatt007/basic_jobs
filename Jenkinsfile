@Library('basic-library') _

pipeline {
  agent 'any'
  options {
    buildDiscarder(logRotator(numToKeepStr: '5'))
  }
  stages {
      stage ('Env') {
          steps {
              sh 'env'
              sayHello 'Vatsal'
          }
      }
  }
  post {
    always {
      cleanWs()
    }
  }  
}
