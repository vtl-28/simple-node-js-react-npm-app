pipeline {
    agent {
        docker {
            image 'node:20.11.0-alpine3.19'
            label 'docker-agent' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}