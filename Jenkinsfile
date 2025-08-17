pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'yogi', url: 'https://github.com/yogesh773/janrepo.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building the project..."
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying application..."
                // put your deploy script here
            }
        }
    }

    post {
        success {
            echo "✅ Pipeline finished successfully!"
        }
        failure {
            echo "❌ Pipeline failed!"
        }
    }
}

