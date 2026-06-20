pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Downloading Source Code'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t flask-app .'
            }
        }

        stage('Run Container') {
            steps {
                bat 'docker stop flask-container || exit 0'
                bat 'docker rm flask-container || exit 0'
                bat 'docker run -d -p 5000:5000 --name flask-container flask-app'
            }
        }
    }
}