pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/Chapoorvaa/jenkins-nodejs-demo.git'
            }
        }
        stage('Install Dependencies') {
            steps {
            sh 'npm install'
            }
        }
        stage('Run Tests') {
            steps {
            sh 'npm test'
            }
        }
        stage('Build') {
            steps {
            echo 'Build completed successfully'
            }
        }
    }
}