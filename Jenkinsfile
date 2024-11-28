pipeline {
    agent any
    environment {    
        
        
        TEST=credentials("COSIGN_SECRET_KEY") 
    }
    stages {
        stage('test') {
            steps {
                script {
                    echo  credentials("NON_EXISTENT") 
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
