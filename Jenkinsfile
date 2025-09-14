pipeline {
  agent any
  tools { 
        maven 'Maven_3_9_11'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=astar_devsecopswebapp -Dsonar.organization=astar_devsecopswebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=91bd04682a971076d5810a9e471bc7e9c98342e1'
			}
        } 
  }
}
