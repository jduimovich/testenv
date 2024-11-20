pipeline {
    agent any
    environment {      
        TEST_MISSING = credentials('TEST_MISSING')   
        ZZZ="${TEST_MISSING}"
        ZZZ="${NON_EXISTENT}"
    }
    stages {
        stage('test') {
            steps {
                script {
                  sh '''
                    echo "$TEST_MISSING" | wc      
                    echo "$ZZZ" | wc                        
                  '''
                }
            }
        } 

    }
}
