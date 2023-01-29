pipeline {
    agent any

    stages {
        stage('Build Docker image') {
            steps{
                script {
                    dockerapp = docker.build("mauriciomaxuel123/kube-news:${env.BUILD_ID }", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }
}