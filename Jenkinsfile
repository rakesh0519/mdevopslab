pipeline {
    agent any  // Use any available agent for this job

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                // Insert build commands here, e.g., compiling code
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Insert test commands here, e.g., running unit tests
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
                // Insert deploy commands here, e.g., deploying to a server
            }
        }
    }
    
    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
