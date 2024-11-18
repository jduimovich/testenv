



pipeline {
    agent any
    environment {    
        
        TEST123 = credentials('TEST123') 
         
        TRUSTIFICATION_BOMBASTIC_API_URL = credentials('TRUSTIFICATION_BOMBASTIC_API_URL') 
        TRUSTIFICATION_OIDC_ISSUER_URL = credentials('TRUSTIFICATION_OIDC_ISSUER_URL')
        TRUSTIFICATION_OIDC_CLIENT_ID = credentials('TRUSTIFICATION_OIDC_CLIENT_ID')
        TRUSTIFICATION_OIDC_CLIENT_SECRET = credentials('TRUSTIFICATION_OIDC_CLIENT_SECRET')
        TRUSTIFICATION_SUPPORTED_CYCLONEDX_VERSION = credentials('TRUSTIFICATION_SUPPORTED_CYCLONEDX_VERSION')
    }
    stages {
        stage('test') {
            steps {
                script {
                  sh '''
                    pwd
                    ls -al  
                    echo "SIZE OF TEST123
                    echo "$TEST123" | wc  
                    echo 
                    bash showenv 
                     
                  '''
                }
            }
        } 

    }
}
