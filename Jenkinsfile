pipeline {
    agent any
    environment {     
        TEST=credentials("COSIGN_SECRET_KEY") 
    }
    stages {
        stage('test') {
            steps {
                script {
                    import jenkins.*
                    import jenkins.model.* 
                    import hudson.*
                    import hudson.model.*
                    def jenkinsCredentials = com.cloudbees.plugins.credentials.CredentialsProvider.lookupCredentials(
                            com.cloudbees.plugins.credentials.Credentials.class,
                            Jenkins.instance,
                            null,
                            null
                    );
                    for (creds in jenkinsCredentials) {
                        println(jenkinsCredentials.id)
                    }
                    
                    echo  "Hello" 
        
                }  
            }
        } 
    }
}
