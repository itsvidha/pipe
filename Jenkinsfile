pipeline {
    agent any 
    environment {
        course = "Devops mastery"
        name = "Siva" 
    }
    stages {
        stage ('Build') {
            environment {
                cloud = "GCP"   
            }
            steps {
                echo "Welcome ${name}"
                echo "You enrolled for ${course} course"
                echo "You are certified in ${cloud} course"
            }
        }
        stage ('secondstage'){
            steps {
                echo "Welcome ${name}"
                echo "You enrolled for ${course} course"
                echo "You are certified in ${cloud} course"
            }
        }
    }
}
