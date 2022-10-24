pipeline {
    agent any

    stages {
        stage ('Build Docker Image') {
            steps {
                script {
                    deckerapp = docker.build("aloysioc/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }

}