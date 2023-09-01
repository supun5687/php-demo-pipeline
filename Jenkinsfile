pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Check out the code from a Git repository
                echo 'CHECKOUT'
            }
        }

        stage('Build') {
            steps {
                // Build your code (you can replace this with your build tool)
                echo 'BUILD application'
            }
        }

        stage('Test') {
            steps {
                // Run your tests (you can replace this with your testing framework)
                echo 'TEST application'
            }
        }

        stage('Deploy to Test') {
            steps {
                // Deploy the code to a test environment
                echo 'DEPLOY application'
            }
        }
    }
}
    
