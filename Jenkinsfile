pipeline {
   agent any

   stages {
      stage('Upload Zip To Nexus'){
            steps{
                script{

                    nexusArtifactUploader artifacts: [
                        [
                            artifactId: 'myZip', 
                            classifier: '', 
                            file: "myZip", 
                            type: 'zip'
                        ]
                    ], 
                    credentialsId: 'nexus3', 
                    groupId: 'com.repo', 
                    nexusUrl: '10.79.244.15:8081', 
                    nexusVersion: 'nexus3', 
                    protocol: 'http', 
                    repository: 'MyFirstNuget', 
                    version: "1" 
                    
                  /*  nexusArtifactUploader (
                    credentialsId: 'nexus3', 
                    groupId: 'com.repo',
                    nexusUrl: '10.79.244.15:8081', 
                    nexusVersion: 'nexus3', 
                    protocol: 'http', 
                    repository: 'MyFirstNuget', 
                    version: '1'); */

                    
                    }
            }
        }
   }
}
