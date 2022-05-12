pipeline {
  agent 'any'
  options {
    buildDiscarder(logRotator(numToKeepStr: '5'))
  }
  stages {
      stage ('Env') {
          steps {
              sh 'env'    
          }
      }
  }
  post {
    always {
      cleanWs()
    }
  }  
}
