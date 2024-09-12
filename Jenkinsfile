pipeline {
    agent any 
    stages {
        stage ('Build') {
            steps {
                echo "Welcome to Build Stage"
            }
        }
        stage ('Depkoy to dev') {
            steps {
                echo "Deploying to dev environment"
            }
        }
        stage ('Deploy to Stage') {
            when {
                expression {
                    // stage should execute with either production branch or staging branch
                    BRANCH_NAME ==~ /(production|staging)/
                }
            }
            steps {
                echo "Deploying to Stage Environment "
            }
        }
    }
}
