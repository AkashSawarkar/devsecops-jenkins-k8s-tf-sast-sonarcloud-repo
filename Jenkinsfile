pipeline {
  agent any
  tools { 
        maven 'Maven_3_9_11'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=astar_devsecops -Dsonar.organization=astar_devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=a5f36553e21834542540247d415707933228f7d1'
			}
        } 
  }
}
