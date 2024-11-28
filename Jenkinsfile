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
          try { 
                sh '''    
                    echo "hhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhh" 
                  '''
          } catch (Exception e) {
              echo 'Exception occurred: ' + e.toString()
                sh '''    
                    echo "zzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzz" 
                  '''
          }
        }
                
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
