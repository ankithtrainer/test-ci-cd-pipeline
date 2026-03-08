pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/ankithtrainer/test-ci-cd-pipeline'
            }
        }

        stage('Build') {
            steps {
                echo "Building application..."
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }

        stage('Deploy') {
            steps {
                bat 'mkdir C:\\deploy-demo'
                bat 'copy index.html C:\\deploy-demo'
            }
        }
    }
}