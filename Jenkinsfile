pipeline {
    agent any 
    stages {
        stage ('hello'){
            steps {
                echo "hello !!!!"
            }
        }
        stage ('sricptstage'){
            steps {
                script {
                    def course = "k8s"
                    if (course == 'k8s')
                      println("Thanks for enrolling to ${course}")
                    else 
                      println ("Do enroll")
                    //sleep 60 // seconds
                    echo "Script block ended here"
                }
            }
        }
    }
}
