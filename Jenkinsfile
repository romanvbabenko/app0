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
                echo 'Testing ...'
            }
        }
        
        stage('QA') {
            steps {
                input 'Do u approve the build?';
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploing ...'
            }
        }
    }
}
