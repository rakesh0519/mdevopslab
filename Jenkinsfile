pipeline {
    agent any
    
    environment {
        // Define environment variables with paths relative to Jenkins home
        HOME_DIR = '/var/lib/jenkins'
        WORKSPACE_DIR = "${HOME_DIR}/workspace/myproject"
        DEPLOY_DIR = "${HOME_DIR}/deployments"
    }

    stages {
        stage('Build') {
            steps {
                // Use environment variables in commands
                sh 'echo Building project in workspace: $WORKSPACE_DIR'
                // Example build command:
                // sh "cd $WORKSPACE_DIR && ./build_script.sh"
            }
        }

        stage('Test') {
            steps {
                sh 'echo Running tests in workspace: $WORKSPACE_DIR'
                // Example test command:
                // sh "cd $WORKSPACE_DIR && ./test_script.sh"
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo Deploying to directory: $DEPLOY_DIR'
                // Example deploy command:
                // sh "cp -r $WORKSPACE_DIR/build/* $DEPLOY_DIR/"
            }
        }
    }

    post {
        success {
            sh 'echo Pipeline completed successfully!'
        }
        failure {
            sh 'echo Pipeline failed.'
        }
    }
}
