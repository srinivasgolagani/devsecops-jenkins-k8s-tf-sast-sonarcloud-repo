pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=1securityguru -Dsonar.organization=1securityguru -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=2cee1ba992394175de74b88125a7bf43d8f21a73'
			}
        } 
  }
}
