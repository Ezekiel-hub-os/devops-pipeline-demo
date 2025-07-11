pipeline {
    agent {
        docker { image 'python:3.10' }  // מריץ בתוך קונטיינר עם פייתון
    }

    stages {
        stage('Clone Repo') {
            steps {
                echo 'Cloning repository...'
            }
        }

        stage('Install Requirements') {
            steps {
                echo 'Installing requirements...'
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Run App') {
            steps {
                echo 'Running app...'
                sh 'python app.py'
            }
        }
    }
}

