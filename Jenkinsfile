pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        parallel(
          "Build": {
            sh 'sh color.sh'
            
          },
          "encodedName": {
            sh 'echo "\033[32m some text \033[0m"'
            
          }
        )
      }
    }
  }
}