pipeline {
  agent any
  tools { 
        maven 'Maven_3_9_11'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=astar_devsecops -Dsonar.organization=astar_devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=b2c1dda32f4f1153c62631ee63770968f88079f0'
			}
        } 
  }
}
