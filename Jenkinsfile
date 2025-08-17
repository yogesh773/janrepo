pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/yogesh773/lab_ducat.git
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
OAOAOA            }
        }
OAOAOAOAOAOAOAOAOAOA    }
OA
    post {
OAOAOA        success {
OA            echo "✅ Pipeline finished successfully!"
OA        }
        failure {
            echo "❌ Pipeline failed!"
OAOAOAOAOAOAOAOAOA        }
OA    }
OA}

