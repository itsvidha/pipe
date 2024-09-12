pipeline {
    agent any 
    environment {
        DEPLOY_TO = 'production' // this is static, we shall see about dynamic in parameter section
    }
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
                allOf {
                    // the below all conditions should be satisfied inorder for this stage tot execute
                    branch 'production'
                    environment name: 'DEPLOY_TO', value: 'production'
                }
            }
            steps {
                echo "Deploying to Stage Environment "
            }
        }
    }
}
