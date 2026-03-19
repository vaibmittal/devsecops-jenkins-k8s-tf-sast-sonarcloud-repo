pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp786 -Dsonar.organization=asgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=66db92f44b9d50744e7de4167de231ca40e88d78'
			}
        } 
  }
}
