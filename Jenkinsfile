pipeline {
    agent {
        docker {
            image 'node:latest'
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'yarn install' 
            }
        }
        stage('Test & Coverage') {
            steps {
                sh 'yarn test --coverage' 
            }
        }
    }
}