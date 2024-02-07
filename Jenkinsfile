pipeline {

	agent any
	
	stages {
		
		stage("Build") {

			tools {
				maven 'Maven 3.9.6'
			}
			steps {

				sh 'mvn clean build'
			}
		}
		
		stage("Test") {

			steps {

				withMaven {
	
					sh 'mvn test'
				}
			}
		}
	}
}
