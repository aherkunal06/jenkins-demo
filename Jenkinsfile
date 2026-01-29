pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                echo 'Pulling code from GitHub'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage running'
                sh 'ls -la'
            }
        }

        stage('Test') {
            steps {
                echo 'No tests yet'
            }
        }
    }
}
