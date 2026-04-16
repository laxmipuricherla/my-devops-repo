stage('Deploy') {
    steps {
        sh '''
        echo "Restarting service..."
        sudo systemctl restart myapp
        sudo systemctl status myapp
        '''
    }
}
