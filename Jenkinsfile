pipeline {
  agent any
  tools { 
        maven 'Maven_3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=232nycewebapp -Dsonar.organization=232nycewebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=6daca4246d6bdc8a9121bb679067513bee52a22b'
			}
        } 
  }
}
