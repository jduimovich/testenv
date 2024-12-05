@Library('RHTAP_Jenkins@v1.3') _

pipeline {
    agent any
    environment {     
        TEST=credentials("COSIGN_SECRET_KEY") 
    }
    stages {
        stage('test') {
            steps { 
                script  {  
                     sh  '''
                          curl https://raw.githubusercontent.com/redhat-appstudio/tssc-sample-sbom-scans/refs/heads/main/live-demo
                        '''
                    }
                }
            }
        }
    }
