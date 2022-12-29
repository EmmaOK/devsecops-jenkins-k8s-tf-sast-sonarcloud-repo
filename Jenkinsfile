pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=hgbuggywebapp -Dsonar.organization=hgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=2766b952001571bfa489895ac3c0096582a74295'
			}
        } 
  }
}
