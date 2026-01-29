pipeline {
    agent any

    environment {
        APP_NAME = "jenkins-demo"
        ENV_NAME = "dev"
    }

    stages {
        stage('Checkout Code') {
            steps {
                echo "App: ${APP_NAME}"
                echo "Environment: ${ENV_NAME}"
                checkout scm
            }
        }

        stage('Build') {
            steps {
                sh 'ls -la'
            }
        }
    }
}
