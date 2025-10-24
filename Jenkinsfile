pipeline {
    agent any

    stages {
        stage('Pull Source Code') {
            steps {
                git branch: 'main', url: 'https://github.com/octoabrian/e-voting-app.git'
            }
        }
     stage('Build Container Image') {
            steps {
                sh 'docker compose build'
            }
        }  
     stage('Deploy Container Apps') {
            steps {
                echo 'docker compose push'
            }
        }
     stage('Push Image') {
            steps {
                echo 'Push Image'
            }
        }
    }
}