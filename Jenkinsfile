pipeline {

    agent any

    stages {

        stage('Checkout') {
            steps {
                 checkout scm
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
