pipeline {
    agent any
    environment{
        DEPLOY_TO = "prod"
    }
    stages{
        stage('deploy')
        {
            when{
                environment name : "DEPLOY_TO", value: "prod"
            }
            steps{
                echo "deploying"
            }
        }
    }
}
