

pipeline {
    agent any
    environment {     
        TEST=credentials("COSIGN_SECRET_KEY") 
    }
    stages {
        stage('test') {
            steps {
                echo "Pre-Script" 
                script  { 
                    echo "In-Script" 
                    try {  
                        echo "In-Try" 
                        withCredentials(bindings: [sshUserPrivateKey(credentialsId: 'COSIGN_SECRET_KEY', \
                                                                     keyFileVariable: 'SSH_KEY_FOR_ABC')]) {
                        sh  '''
                            echo "In withCredentials"
                           `export AAA=666
                            echo "InWC AAA $AAA"
                           '''
                        }
                        echo "after withCredentials" 
                    } catch (all) { 
                        echo "Error" 
                    }
                    echo "Next" 
                     sh  '''
                           echo $AAA
                           '''
                    }
                }
            }
        }
    }
