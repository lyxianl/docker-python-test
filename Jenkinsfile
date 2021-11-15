pipeline {
    agent {
        dockerfile {
            filename 'Dockerfile'
            label 'my-defined-label'
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