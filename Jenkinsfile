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
            sleep 6
            
          },
          "c": {
            sleep 8
            
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
