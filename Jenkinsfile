pipeline {
  agent any
  tools { 
        maven 'Maven_3_9_11'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=astar_devsecops1 -Dsonar.organization=astar_devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=465dd4aca5c413ea7019cc1a1ba6947724312c73'
			}
        } 
  }
}
