pipeline {
    agent any
    stages {
        stage('Deploy with Helm') {
            steps {
                script {
                    sh '/c/ProgramData/chocolatey/bin/helm upgrade --install my-webapp ./webapp --namespace default'
                }
            }
        }
    }
}