pipeline {
    agent {
        dockerfile {
            filename 'Dockerfile'
            label 'linux-agent-any'
            args '-t test-docker'
        }
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