pipeline {
    agent any
    stages {
        stage('Clone Repo') {
            steps {
                echo 'Cloning repository...'
                // אפשר להוסיף git clone אם תשתמש ב-GitHub
            }
        }
        stage('Install Requirements') {
            steps {
                echo 'Installing requirements...'
                sh 'pip3 install -r requirements.txt || true'
            }
        }
        stage('Run App') {
            steps {
                echo 'Running app...'
                sh 'python3 app.py'
            }
        }
    }
}

