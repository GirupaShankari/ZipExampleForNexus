pipeline {
   agent any

   stages {
      stage('Upload Zip To Nexus'){
            steps{
                script{

                   nexusArtifactUploader artifacts: [
                        [
                            artifactId: 'Installation of Nexus Repository on Windows.zip', 
                            classifier: '', 
                            file: "Installation of Nexus Repository on Windows.zip", 
                            type: 'zip'
                        ]
                    ], 
                    credentialsId: 'nexus3', 
                    groupId: 'com', 
                    nexusUrl: '10.79.244.15:8081', 
                    nexusVersion: 'nexus3', 
                    protocol: 'http', 
                    repository: 'MyFirstNuget', 
                    version: "1" 
                   
                  /*  nexusArtifactUploader artifacts: [
                        [
                            artifactId: 'mySecondZipFile', 
                            classifier: '', 
                            file: "Installation of Nexus Repository on Windows.zip", 
                            type: 'zip'
                        ]
                    ], 
                    credentialsId: 'nexus3', 
                    groupId: 'in.javahome', 
                    nexusUrl: '10.79.244.15:8081', 
                    nexusVersion: 'nexus3', 
                    protocol: 'http', 
                    repository: 'simpleapp-release', 
                    version: "1" */
                    
                    
                    }
            }
        }
   }
}
