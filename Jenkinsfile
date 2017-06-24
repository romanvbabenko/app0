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
                input 'Do you approve the branch?'
            }
        }
        
        stage('Done') {
            steps {
                echo 'done'
            }
        }
    }
}
