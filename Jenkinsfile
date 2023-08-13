pipeline {
    agent {
        node {
            label 'devops1'
        }
    }

    stages {
        stage('Build Apps') {
            steps {
                sh 'npm install';
            }
        }
        stage('Testing') {
            steps {
                sh '''npm test
                npm run test:coverage'''
            }
        }
        stage('Scanning Code') {
            steps {
                sh '''
                sonar-scanner   -Dsonar.projectKey=training-devops   -Dsonar.sources=.   -Dsonar.host.url=http://10.23.2.3:9000   -Dsonar.login=sqp_8545265cb180ed2d322be5ae85b72aa6305cfb7a
                '''
            }
        }
        stage('Build Image') {
            steps {
                echo 'Build Image'
            }
        }
        stage('Deploy Apps') {
            steps {
                echo 'Deploy Apps'
            }
        }
        stage('Push Image') {
            steps {
                echo 'Push image'
            }
        }
    }
}