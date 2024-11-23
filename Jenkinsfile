library identifier: 'RHTAP_Jenkins@dev', retriever: modernSCM(
  [$class: 'GitSCMSource',
   remote: 'https://github.com/jduimovich/tssc-sample-jenkins.git'])




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
                    echo "$ZZZZZ" | base64  
                  '''
                }
            }
        } 

    }
}
