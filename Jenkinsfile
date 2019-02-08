pipeline {
    agent { docker  { image 'python:3.5.1' 
                      args '-u root -v /var/run/docker.sock:/var/run/docker.sock'  } }
    stages {
        stage('first') {
            steps {
                sh 'python --version'
            }
        }
    }
}
