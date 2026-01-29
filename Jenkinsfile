pipeline {
    agent any

    environment {
        APP_NAME = "jenkins-demo"
        DEPLOY_DIR = "/var/www/jenkins-demo"
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                sh 'ls -la'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                  echo "Deploying application..."
                  cp index.html $DEPLOY_DIR/
                  echo "Deployment complete"
                '''
            }
        }
    }
}

