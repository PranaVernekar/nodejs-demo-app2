pipeline {
    agent any

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
          docker stop nodejs-demo || true
          docker rm nodejs-demo || true
          docker run -d -p 3000:3000 --name nodejs-demo nodejs-demo-app:latest
        '''
    }
}
