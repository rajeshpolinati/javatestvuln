pipeline {
    agent any
  	  
    stages {
        stage('ZIP directory to be uploaded or unzip something') {
            agent {
                docker {
                    image 'javieraviles/zip'
                    reuseNode true
                }
            }
            steps {
                echo "Creating zip file..."
	    
                sh "zip -r 'FODJenkinsPOC.zip' '/var/jenkins_home/workspace/Cloud-Brokerage/jenkins_FOD_POC/'"
            }
        
        }
    }
}
