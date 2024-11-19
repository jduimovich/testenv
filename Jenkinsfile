pipeline {
    agent any
    environment {          
        try {
            TEST_MISSING = credentials('TEST_MISSING') 
        }
        catch(all) {
             TEST_MISSING="its missing"
        } 
    }
    stages {
        stage('test') {
            steps {
                script {
                  sh '''
                    echo "$TEST_MISSING" | wc                         
                  '''
                }
            }
        } 

    }
}
