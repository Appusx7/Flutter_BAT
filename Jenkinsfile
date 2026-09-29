pipeline {
    agent any

    environment {
        PATH = "C:\\src\\flutter\\bin;${env.PATH}"
    }

    stages {
        stage('Get Dependencies') {
            steps {
                bat 'flutter pub get'
            }
        }

        stage('Test') {
            steps {
                bat 'flutter test'
            }
        }

        stage('Build Web') {
            steps {
                bat 'flutter build web'
            }
        }
    }
}