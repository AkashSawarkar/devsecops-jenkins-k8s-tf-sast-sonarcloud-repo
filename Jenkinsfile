pipeline {
  agent any
  tools { 
        maven 'Maven_3_9_11'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=astar_devsecopswebapp -Dsonar.organization=astar_devsecopswebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=e81b603607cd943afe7afb637b95da3e4b53f633'
			}
        } 
  }
}
