pipeline {
    agent { docker  { image 'python:3.5.1' } }
    stages {
        stage('first') {
            steps {
                sh 'python --version'
            }
        }
    }
}