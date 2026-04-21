pipeline {
    agent {
        docker {
            image 'node:18'
        }
    }

    stages {

        stage('Install') {
            steps {
                sh 'npm install'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                nohup node app.js > output.log 2>&1 &
                '''
            }
        }
    }
}
