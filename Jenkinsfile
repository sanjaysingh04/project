pipeline {
    agent { label 'slave' }  // Run the build on the slave node

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/sanjaysingh04/project.git'
            }
        }
        
        stage('Build') {
            steps {
                sh 'echo "Building the application..."'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Deploying application..."'
            }
        }
    }
}
