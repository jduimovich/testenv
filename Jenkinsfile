pipeline {
    agent any
    environment {          
        YYY="${NON_EXISTENT}"
    }
    stages {
        stage('test') {
            steps {
                script {
                  sh '''   
                    echo "$YYY" | wc                        
                  '''
                }
            }
        } 

    }
}
