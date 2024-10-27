pipeline {
    agent any  // Use any available agent for this job

    stages {
        stage('Build') {
            steps {
                // Replace with actual build commands
                sh 'echo Building the project...'
                // For example, a Java build command might be:
                // sh './gradlew build'
            }
        }

        stage('Test') {
            steps {
                // Replace with actual test commands
                sh 'echo Running tests...'
                // For example, to run tests:
                // sh './gradlew test'
            }
        }

        stage('Deploy') {
            steps {
                // Replace with actual deployment commands
                sh 'echo Deploying the project...'
                // For example, to deploy:
                // sh './deploy_script.sh'
            }
        }
    }

    post {
        success {
            // Message on success
            sh 'echo Pipeline completed successfully!'
        }
        failure {
            // Message on failure
            sh 'echo Pipeline failed.'
        }
    }
}
