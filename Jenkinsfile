pipeline {
    agent any
    stages {
        stage('Echo') {
            steps {
                sh('''
                docker images -a
                docker build -t test-image:latest .
                docker images -a
                ''')
            }
        }
    }
}