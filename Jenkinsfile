pipeline {
    agent any
    stages {
        stage('Echo') {
            steps {
                sh('''
                docker images -a
                docker build -t fromImage:latest .
                docker images -a
                ''')
            }
        }
    }
}