pipeline {
    agent any 
    stages {
        stage ('build'){
            steps {
                retry (3) {
                    echo "Welcome to jenkins"
                    // error "testing retry"
                }
                echo "After retry block"
            }
        }
    }
}
