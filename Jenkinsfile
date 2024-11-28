pipeline {
    agent any
    environment {          
        TEST="${NON_EXISTENT}"
        TEST2="${NON_EXISTENT2}"
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
