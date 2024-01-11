pipeline {
    agent any

    stages {
        stage('Display Branch Name') {
            steps {
                script {
                    // Get the current branch name
                    def branchName = env.BRANCH_NAME ?: 'Not available'

                    // Display the branch name
                    echo "Current Branch: ${branchName}"
                }
            }
        }

        // Add more stages as needed for your build/test/deployment steps
        stage('Build') {
            steps {
                echo 'Building...'
                // Add your build steps here
            }
        }

        // Add more stages as needed

    }
}
