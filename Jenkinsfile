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
                sh 'docker build -t jenkins-docker-demo:v1 .'
            }
        }

        stage('Display Image Details') {
            steps {
                sh 'docker images jenkins-docker-demo:v1'
            }
        }
    }
}
