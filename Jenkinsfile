pipeline {
    agent any 
    stages {
        stage ('Build') {
            steps {
                timeout (time: 300, unit:'SECONDS'){ // 5min approval.....s
                    input message: 'Are you Building the applicaiton', ok: 'yes', submitter: 'dhanush,vijju'
                }
                echo "Builing the applicaiton"
            }
        }
    }
}
