pipeline {
    agent any
    parameter{
        string(name: 'PERSON',  defaultValue: 'Dhanush', description: 'Please Enter your name')
        string (name: 'BRANCH_NAME', defaultValue: "main", description: 'Whats the branch i should build??') 
        booleanParam(name: 'DEBUG_BUILD', defaultValue: true, description: 'toogle this value')
        choice(name: 'ENV', choices: ['dev', 'tst', 'stg', 'prd'], description: 'choose an environment')   
    }
    stages{
        stage('Example'){
            steps{
                echo "welcome mr.${params.PERSON}"
                echo "Boolean parameter is: ${params.TOOGLE}"
                echo "Deploying to ${params.ENV} environment"
            }

        }
    }

               }
