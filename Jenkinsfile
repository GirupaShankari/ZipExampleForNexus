pipeline {
   agent any

   stages {
      stage('Upload Zip To Nexus'){
            steps{
                script{

                   /* nexusArtifactUploader artifacts: [
                        [
                            artifactId: 'simple-app', 
                            classifier: '', 
                            file: "target/simple-app-2.0.0.war", 
                            type: 'zip'
                        ]
                    ], 
                    credentialsId: 'nexus3', 
                    groupId: 'com.repo', 
                    nexusUrl: '10.79.244.15:8081', 
                    nexusVersion: 'nexus3', 
                    protocol: 'http', 
                    repository: 'MyFirstNuget', 
                    version: "1" */
                    
                    nexusArtifactUploader (
                    credentialsId: 'nexus3', 
                    groupId: 'com.repo',
                    nexusUrl: '10.79.244.15:8081', 
                    nexusVersion: 'nexus3', 
                    protocol: 'http', 
                    repository: 'MyFirstNuget', 
                    version: '1');
                    
                    }
            }
        }
   }
}
