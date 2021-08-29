pipeline {
    agent {
        docker {
            image 'node:12.12.0'
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
