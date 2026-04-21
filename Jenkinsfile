pipeline {
    agent any

    tools {
        nodejs "NodeJS"
    }

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                url: 'https://github.com/snehasuman019/CI-CD-Pro.git'
            }
        }

        stage('Install') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                sh 'echo Build Successful'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo Deployment Successful'
            }
        }
    }
}
