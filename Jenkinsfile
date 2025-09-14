pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_11'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=astar_devsecopswebapp -Dsonar.organization=astar_devsecopswebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=4ab574272b347c3cd239a8f91c309dba55f5a1dc'
			}
        } 
  }
}
