pipeline{
	agent any

	tools{
		maven 'Maven3.6.3'
	}
	
	stages{
		stage('build'){
			steps{
				sh 'mvn compile'
			}
		}
	}	
	
	stages{
		stage('test'){
			steps{
				sh 'mvn clean test'
			}
		}
	}	
	
	stages{
		stage('package'){
			steps{
				sh 'mvn package -DskipTests'
			}
		}

	}	
}
