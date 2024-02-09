pipeline {

	agent any
	
	tools {
		
		maven 'Maven 3.9.6'
	}
	
	stages {
		
		stage("Build") {

			steps {

				sh 'mvn clean generate-sources'
			}
		}
		
		stage("Test") {

			steps {

				sh 'mvn package'
			}
		}
	}
}
