pipeline {
    agent {
        docker {
            image 'python:3.12'
            args '-u root'
        }
    }

    stages {
        stage('Install dependencies') {
            steps {
                sh '''
                    pip install --upgrade pip
                    pip install -r requirements.txt
                '''
            }
        }

        stage('Run Django tests') {
            steps {
                sh '''
                    python manage.py test
                '''
            }
        }
    }
}