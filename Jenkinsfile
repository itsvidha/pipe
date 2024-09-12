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
                anyOf {
                    // any of the below condition can be satisifed for this stage to be executed 
                    branch 'stage'
                    environment name: 'DEPLOY_TO', value: 'production'
                }
            }
            steps {
                echo "Deploying to Stage Environment "
            }
        }
    }
}
