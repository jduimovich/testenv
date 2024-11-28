
pipeline {
    agent any
    environment {     
        TEST=credentials("COSIGN_SECRET_KEY") 
    }
    stages {
        stage('test') {
            steps {
                script  { 
                try { 
                    withCredentials(bindings: [sshUserPrivateKey(credentialsId: 'jenkins-ssh-key-for-abc', \
                                                                 keyFileVariable: 'SSH_KEY_FOR_ABC')]) {
                    }
                    } catch (all) { 
                        echo "Error" 
                    }
                }
                
            }
        }
    }
}
