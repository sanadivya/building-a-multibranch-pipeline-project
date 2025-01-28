pipeline {
    agent any
    environment{
        CI = 'true'
    }
    tools {
        nodejs 'NODEJS' // Name of the Node.js configuration in Jenkins
    }
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }

        stage('Test') {
            steps {
                bat './jenkins/scripts/test.bat'
            }
        }
    }
}
