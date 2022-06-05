pipeline {
    agent any

    stages {
        stage('confirm version') {
            steps {
                nodejs('nodejs17.9.0') {
                    sh 'node -v'
                    sh 'npm -v'
                }
            }
        }
        stage('install node packages') {
            steps {
                nodejs('nodejs17.9.0') {
                    sh 'npm install'
                }
            }
        }
    }
}
