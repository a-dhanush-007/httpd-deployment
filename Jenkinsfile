pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/your-username/httpd-deployment.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t my-httpd-image .'
            }
        }

        stage('Deploy to Docker') {
            steps {
                sh 'chmod +x deploy.sh && ./deploy.sh'
            }
        }
    }
}

