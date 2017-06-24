pipeline {
    agent any

    stages {
        stage 'Deploy' {
            node {
              echo 'deploying...'
            }
        }      
        
        stage('QA') {
            steps {
                input 'Do you approve the branch?'
            }
        }
        
        stage('Done') {
            steps {
                node {
                    echo 'done'
                }
            }
        }
    }
}
