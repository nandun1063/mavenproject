pipeline {
    agent any
    stages{
        stage('Build'){
            steps{
                sh '/opt/apache-maven-3.5.2/bin/mvn clean package'
                sh "docker build . -t tomcatwebapp:${env.BUILD_ID}"
            }
        }
    } 	 	
}
    
