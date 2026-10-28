
pipeline {
    agent any

    stages {
        stage('Report Build Information') {
            steps {
                echo '===== MULTIBRANCH PIPELINE ====='
                echo "Job Name: ${env.JOB_NAME}"
                echo "Build Number: ${env.BUILD_NUMBER}"
                echo "Branch Name: ${env.BRANCH_NAME}"
                echo "Git Branch: ${env.GIT_BRANCH}"
                echo "Git Commit: ${env.GIT_COMMIT}"
                echo "Workspace: ${env.WORKSPACE}"

                bat 'git branch --show-current'
            }
        }
    }
}
