pipeline {
    agent any
    environment {          
        TEST="${NON_EXISTENT}"
    }
    stages {
        stage('test') {
            steps {
                script {
                  sh '''    
                    echo "$TEST" | base64  
                  '''
                }
            }
        } 

    }
}
