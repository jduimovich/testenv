/* Generated from templates/gitops-template/Jenkinsfile.njk. Do not edit directly. */

library identifier: 'RHTAP_Jenkins@main', retriever: modernSCM(
  [$class: 'GitSCMSource',
   remote: 'https://github.com/redhat-appstudio/tssc-sample-jenkins.git'])

pipeline {
    agent any
    environment {  
        /* URL of the BOMbastic api host (e.g. https://sbom.trustification.dev) */
        TRUSTIFICATION_BOMBASTIC_API_URL = credentials('TRUSTIFICATION_BOMBASTIC_API_URL')
        /* URL of the OIDC token issuer (e.g. https://sso.trustification.dev/realms/chicken) */
        TRUSTIFICATION_OIDC_ISSUER_URL = credentials('TRUSTIFICATION_OIDC_ISSUER_URL')
        TRUSTIFICATION_OIDC_CLIENT_ID = credentials('TRUSTIFICATION_OIDC_CLIENT_ID')
        TRUSTIFICATION_OIDC_CLIENT_SECRET = credentials('TRUSTIFICATION_OIDC_CLIENT_SECRET')
        TRUSTIFICATION_SUPPORTED_CYCLONEDX_VERSION = credentials('TRUSTIFICATION_SUPPORTED_CYCLONEDX_VERSION')
    }
    stages {
        stage('test') {
            steps {
                script {
                    sh "showenv"
                }
            }
        } 

    }
}
