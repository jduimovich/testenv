



pipeline {
    agent any
    environment {   
        
        ROX_API_TOKEN = credentials('ROX_API_TOKEN')
        ROX_CENTRAL_ENDPOINT = credentials('ROX_CENTRAL_ENDPOINT')
        GITOPS_AUTH_PASSWORD = credentials('GITOPS_AUTH_PASSWORD')
        /* Uncomment this when using Gitlab */
        /* GITOPS_AUTH_USERNAME = credentials('GITOPS_AUTH_USERNAME') */
        QUAY_IO_CREDS = credentials('QUAY_IO_CREDS')
        COSIGN_SECRET_PASSWORD = credentials('COSIGN_SECRET_PASSWORD')
        COSIGN_SECRET_KEY = credentials('COSIGN_SECRET_KEY')
        COSIGN_PUBLIC_KEY = credentials('COSIGN_PUBLIC_KEY')
        
        TEST = 123
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
                    echo "hi"
                    echo "$TEST"
                    echo "$TRUSTIFICATION_BOMBASTIC_API_URL" | wc 
                    echo "$TRUSTIFICATION_OIDC_ISSUER_URL" | wc 
                    echo "$TRUSTIFICATION_OIDC_CLIENT_ID" | wc 
                    echo "$TRUSTIFICATION_OIDC_CLIENT_SECRET" | wc 
                    echo "$TRUSTIFICATION_SUPPORTED_CYCLONEDX_VERSION" | wc 
                    env 
                  '''
                }
            }
        } 

    }
}
