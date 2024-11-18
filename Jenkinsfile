



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
                    
                    echo "Testing for 123 or 321 "
                    if [[ "TEST123" == "123" ]]; then
                        echo "---------------------------------"
                        echo "1 2 3"
                        echo "1 2 3"
                        echo "1 2 3"
                        echo "1 2 3"
                        echo "---------------------------------" 
                    fi                     
                    if [[ "TEST123" == "321" ]]; then
                        echo "---------------------------------"
                        echo "3 2 1"
                        echo "3 2 1"
                        echo "3 2 1"
                        echo "3 2 1" 
                        echo "---------------------------------" 
                    fi  
                    echo "$TEST123" | wc  
                     
                  '''
                }
            }
        } 

    }
}
