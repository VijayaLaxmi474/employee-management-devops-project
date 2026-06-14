pipeline {

    agent any

    stages {

        stage('Checkout') {
            steps {
                git url: 'https://github.com/VijayaLaxmi474/employee-management-devops-project.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t employee-app:v1 .'
            }
        }

        stage('Show Docker Images') {
            steps {
                sh 'docker images'
            }
        }

    }
}
