pipeline {
    agent {
        dockerfile true
        args '-t test-docker'
    }
    stages {
        stage('Echo') {
            steps {
                sh('''
                echo `env`
                ls -ra
                ''')
            }
        }
    }
}