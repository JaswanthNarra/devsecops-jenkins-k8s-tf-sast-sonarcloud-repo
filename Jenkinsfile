pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops-buggywebapp -Dsonar.organization=devsecops-buggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=8f3bea0145213aff42bbed5124daa0fdac4b987c'
			}
        } 
  }
}
