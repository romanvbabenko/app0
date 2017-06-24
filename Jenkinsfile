pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        
        staage('QA') {
            steps {
                input 'Do you approve the branch?'
                echo 'Has been approved by QA'
            }
        }
        
        stage('Deploy') {
            steps {
                input 'Do you approve deployment?'
                echo 'Deploying....'
            }
        }
    }
}
