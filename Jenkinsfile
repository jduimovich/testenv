pipeline {
    agent any
    environment {          
        TEST=credentials("COSIGN_SECRET_KEY") 
        TEST2="${COSIGN_SECRET_KEY}" 
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
