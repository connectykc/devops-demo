pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'GitHub Connected'
            }
        }

        stage('Workspace') {
            steps {
                sh 'pwd'
                sh 'ls -la'
            }
        }
    }
}