pipeline {
    agent any

    stages {

        stage('Install') {
            steps {
                sh 'npm install'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                pkill node || true
                nohup node app.js > output.log 2>&1 &
                '''
            }
        }
    }
}
