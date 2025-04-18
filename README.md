pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo "Checking out code..."
            }
        }
        stage('Build') {
            steps {
                echo "Building the project..."
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying to AWS..."
                // Example: sh 'aws s3 cp file.txt s3://aditya-bucket-name/'
            }
        }
    }
}
