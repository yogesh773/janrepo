pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo "📥 Checking out code..."
            }
        }

        stage('Build') {
            steps {
                echo "🔨 Simulating build... (no Maven project found)"
            }
        }

        stage('Test') {
            steps {
                echo "🧪 Running tests..."
            }
        }

        stage('Deploy') {
            steps {
                echo "🚀 Deploying application..."
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
