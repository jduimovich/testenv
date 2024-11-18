



pipeline {
    agent any
    environment {    
        
        TEST1 = credentials('TEST1') 
        TEST2 = credentials('TEST2') 
        TEST3 = credentials('TEST3')  
        TEST3 = credentials('MISSING')  
         
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
                    echo "begin Size of TEST123"
                    echo "$TEST123" | wc  
                    echo "end Size of TEST123"
                    echo 
                    bash showenv 
                     
                  '''
                }
            }
        } 

    }
}
