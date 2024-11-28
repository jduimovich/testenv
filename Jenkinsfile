pipeline {
    agent any
    environment {     
        TEST=credentials("COSIGN_SECRET_KEY") 
    }
    stages {
        stage('test') {
            steps {
                script {
                    echo  "Hello"
                    echo  credentials("NON_EXISTENT") 
        
                }  
            }
        } 
    }
}
