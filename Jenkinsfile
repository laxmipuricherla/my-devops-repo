pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'echo "Build stage running..."'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                echo "Starting web server..."
                nohup python3 -m http.server 8000 > server.log 2>&1 &
                '''
            }
        }
    }
}
