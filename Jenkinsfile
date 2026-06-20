pipeline {
    agent any

    stages {

        stage('GitHub') {
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