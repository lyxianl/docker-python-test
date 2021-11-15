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
        stage('Run') {
            steps {
                sh('''
                docker run --rm -d -p 5050:80 --name test-image --env "FLASK_APP=main.py" test-image:latest > logs.txt 2>&1
                ''')
            }
        }
    }
}