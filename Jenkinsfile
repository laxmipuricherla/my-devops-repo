pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'echo "Build running"'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                echo "Restarting service..."
                sudo systemctl restart myapp
                '''
            }
        }
    }
}
