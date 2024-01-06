pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=kabongongoy_devsecops -Dsonar.organization=kabongongoy -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c9193366c8ff5cc1bea6b8a939736ec327fb2d36'
			}
        } 
  }
}
