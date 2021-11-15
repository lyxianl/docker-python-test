pipeline {
    agent {
        dockerfile true
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