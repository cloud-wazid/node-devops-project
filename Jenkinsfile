pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Code checked out from GitHub'
            }
        }

        stage('Build') {
            steps {
                echo 'Building Node.js application...'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing Node.js application...'
            }
        }

        stage('Docker Build') {
            steps {
                bat 'docker build -t node-devops-app .'
            }
        }

    }
}