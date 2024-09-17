pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/TheWalkingNerd1/Devops_hsy.git', branch: 'main'
            }
        }

        stage('Build') {
            steps {
                dotnet build
            }
        }

    }

    post {
        always {
            cleanWs()
        }
    }
}

