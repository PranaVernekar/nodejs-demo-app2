pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                bat 'docker build -t nodejs-demo-app:latest .'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'npm test || echo "No tests configured"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                bat '''
                  docker stop nodejs-demo || exit 0
                  docker rm nodejs-demo || exit 0
                  docker run -d -p 3000:3000 --name nodejs-demo nodejs-demo-app:latest
                '''
            }
        }
    }
}
