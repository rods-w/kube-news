pipeline {
    agent any

    stages {
        stage ("Build Docker Image") {
            steps {
                script {
                    dockerapp = docker.build("rods-w/kube-news:${env.BUILD_ID}", '-f ./jornada-devops/aula04/kube-news/src/Dockerfile ./jornada-devops/aula04/kube-news/src')
                }
            }
        }    
    }
}
