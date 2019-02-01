pipeline{
	agent any
	stages {
		stage('Build and Unit Test') {
			steps {
				bat '''
					mvn clean install -Dmaven.test.failure.ignore=true
				'''
			}
		} 
	}
}
