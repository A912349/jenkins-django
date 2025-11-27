pipeline {
    agent {
        docker {
            image 'python:latest'
            args '-u root'
        }
    }
    stages {
        stage("Hello") {
            steps {
                sh 'echo Hello_World'

            }
        }
    }
}
