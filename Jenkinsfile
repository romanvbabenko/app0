pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Test') {
            step {
                echo 'Testing ...'
            }
        }
        
        stage('QA') {
            step {
                input 'Do u approve the build?';
            }
        }
        
        stage('Deploy') {
            step {
                echo 'Deploing ...'
            }
        }
    }
}
