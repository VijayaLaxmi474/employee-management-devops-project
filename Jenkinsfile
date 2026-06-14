pipeline {
    agent any

    environment {
        DOCKER_IMAGE = "vijayalaxmi087/employee-app"
    }

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t employee-app .'
            }
        }

        stage('Push Docker Image') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'dockerhub-creds',
                                                  usernameVariable: 'USER',
                                                  passwordVariable: 'PASS')]) {
                    sh '''
                        echo $PASS | docker login -u $USER --password-stdin
                        docker tag employee-app $USER/employee-app:latest
                        docker push $USER/employee-app:latest
                    '''
                }
            }
        }
    }
}
