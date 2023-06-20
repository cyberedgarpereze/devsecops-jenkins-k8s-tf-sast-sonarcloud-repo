pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=cyberbuggywebapp -Dsonar.organization=cyberbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=181a64ddefbf274c35329275d0b8a34780c91a7b'
			}
        } 
  }
}
