pipeline {
  agent any
  tools { 
        maven 'Maven_3_9_11'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=astar_devsecops1 -Dsonar.organization=astar_devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=46ae07e2ad38ab05938eac086c24f2462face8ab'
			}
        } 
  }
}
