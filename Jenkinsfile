pipeline {
    agent any
    environment {          
        TEST=credentials("COSIGN_SECRET_KEY") 
        TEST2=credentials("NON_EXISTENT") 
    }
    stages {
        stage('test') {
            steps {
                script {
                  sh '''    
                    echo "$TEST" | base64  
                    echo "$TEST2" | base64  
                  '''
                }
            }
        } 

    }
}
