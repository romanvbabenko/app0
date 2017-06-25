pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }
    stage('Test') {
      steps {
        parallel(
          "Test": {
            echo 'Testing ...'
            
          },
          "Browser tests": {
            echo 'Testing in Browser'
            
          },
          "Acceptance tests": {
            echo 'Running acceptance tests'
            
          }
        )
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploing ...'
      }
    }
    stage('QA') {
      steps {
        input 'Do u approve the build?'
      }
    }
    stage('Deploy staging') {
      steps {
        echo 'Deploing staging'
        input 'Performance is OK?'
      }
    }
    stage('Merge production') {
      steps {
        echo 'Merging production'
        echo 'Deliting branch'
      }
    }
  }
}