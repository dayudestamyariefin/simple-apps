pipeline {
    agent {
        node {
            label 'devops1'
        }
    }

    stages {
        stage('Build Apps') {
            steps {
                echo 'Build apps'
            }
        }
        stage('Testing') {
            steps {
                echo 'Testing'
            }
        }
        stage('Scanning Code') {
            steps {
                echo 'Scanning Code'
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