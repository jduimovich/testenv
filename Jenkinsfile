pipeline {
    agent any
    environment {          
        ZZZZZ="${NON_EXISTENT}"
    }
    stages {
        stage('test') {
            steps {
                script {
                  sh '''   
                    echo "$ZZZZZ" | wc                        
                  '''
                }
            }
        } 

    }
}
