pipeline {

	agent any
	
	tools {
		
		maven 'Maven 3.9.6'
	}
	
	stages {
		
		stage("Build") {

			steps {

				sh 'mvn clean generate-sources install'
			}
		}
		
		stage("Test") {

			steps {

				sh 'mvn compile'
			}
		}
	}
}
