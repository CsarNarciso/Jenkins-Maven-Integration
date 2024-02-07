pipeline {

	agent any
	
	stages {
		
		stage("Build") {

			tools {
				maven 'Maven 3.9.6'
			}
			steps {

				sh 'mvn --version'
			}
		}
		
		stage("Test") {
			
			withMaven {
	
				sh 'mvn --version'
			}
		}
	}
}
