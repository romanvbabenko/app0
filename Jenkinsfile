pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        echo 'deploying...'
      }
    }
    stage('QA') {
      steps {
        parallel(
          "QA": {
            input 'Do you approve the branch?'
            
          },
          "QA2": {
            input 'QA2 Approve?'
            
          }
        )
      }
    }
    stage('Done') {
      steps {
        echo 'done'
      }
    }
  }
}