pipeline {
  agent any
  stages {
    stage('a') {
      steps {
        parallel(
          "a": {
            sh 'ls'
            
          },
          "b": {
            sleep 60
            
          },
          "c": {
            sleep 10
            
          }
        )
      }
    }
    stage('aa') {
      steps {
        isUnix()
      }
    }
    stage('aaa') {
      steps {
        error 'error1'
      }
    }
  }
}