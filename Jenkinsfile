pipeline {
    agent {
        Dockerfile true
    }
    stages {
        stage('Echo') {
            sh('''
            echo `env`
            ''')
        }
    }
}