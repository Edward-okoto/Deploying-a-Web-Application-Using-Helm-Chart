pipeline {
    agent any
    stages {
        stage('Deploy with Helm') {
            steps {
                withCredentials([file(credentialsId: 'kubeconfig-cred-id', variable: 'KUBECONFIG')]) {
                    bat 'C:\\ProgramData\\chocolatey\\bin\\helm upgrade --install my-webapp C:\\Users\\edwar\\Documents\\Myworkspace\\Deploying-a-Web-Application-Using-Helm-Chart\\helm-web-app\\webapp --namespace default'
                }
            }
        }
    }
}