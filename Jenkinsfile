pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3007:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
        stage('Test') { 
            steps {
                sh 'test.sh' 
            }
        }
    }
}
