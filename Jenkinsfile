pipeline{
	agent any
	stages {
	
		stage ('Pull source code from GIT') {
			steps {
					git 'https://github.com/devops5032883/springboot-crud.git' 
				
			}
		}
		stage('Build and Unit Test') {
			steps {
				bat '''
					mvn clean install
				'''
			}
		} 
	}
}
