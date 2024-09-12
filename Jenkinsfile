pipeline {
    agent any
    environment{
        DEPLOY_TO = "prod"
    }
    stages{
        stage('deploy')
        {
            when{
                not{
                equals expected: 12 , actual: currentBuild.number
                }
            }
            steps{
                echo "deploying"
            }
        }
    }
}
