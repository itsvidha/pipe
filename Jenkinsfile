pipeline {
    agent any
    environment{
        DEPLOY_TO = "prod"
    }
    stages{
        stage('deploy')
        {
            when{
                equals expected: 12 , actual: currentBuild.number
            }
            steps{
                echo "deploying"
            }
        }
    }
}
