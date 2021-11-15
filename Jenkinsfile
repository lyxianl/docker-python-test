pipeline {
    agent {
        docker {
            Dockerfile true
        }
    }
    stages {
        stage('Echo') {
            steps {
                sh('''
                echo `env`
                ''')
            }
        }
    }
}