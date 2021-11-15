pipeline {
    agent {
        dockerfile {
            // filename 'Dockerfile'
            label 'linux-agent-any'
            // args '-t test-docker'
            args '-t lyxian/flask-demo:1'
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