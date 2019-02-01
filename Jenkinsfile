pipeline{
	agent any
	stages {
		stage ('Pull the source code') {
			steps {
					git 'https://github.com/devops5032883/springboot-crud.git' 
				
			}
		}
		
		stage('Build and Unit Test') {
			steps {
				bat '''
					mvn clean install -Dmaven.test.failure.ignore=true
				'''
			}
		} 
	}
}
