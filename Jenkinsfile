pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: '*/main', url: 'https://github.com/jai2003/repo-b.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'make build' // Replace with your actual build command
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'make test' // Replace with your actual test command
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'make deploy' // Replace with your actual deployment command
            }
        }
    }
}
