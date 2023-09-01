pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Check out the code from the Git repository
                checkout scm
            }
        }

        stage('Copy to Docker Container') {
            steps {
                script {
                    // Define your Docker container name
                    def dockerContainerName = 'jenkins-container-php'

                    // Copy the repository to the Docker container
                    sh "docker cp . ${dockerContainerName}:/var/www/html"
                }
            }
        }
    }

    post {
        success {
            // This block of steps will execute if the pipeline is successful
            echo 'Repository copied to Docker container successfully!'
        }

        failure {
            // This block of steps will execute if the pipeline fails
            echo 'Pipeline failed!'
        }

        
    }
}
