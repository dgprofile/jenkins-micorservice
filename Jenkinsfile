pipeline {
	//agent any 
	agent { docker { image 'maven:3.18'} }
	stages {
		stage ('BUILD') {
			steps {
				sh 'mvn --version'
				echo "BUILD" 
			} 
		}
		stage ('TEST') {
			steps { 
				echo "TEST" 
			} 
		}
		stage ('INTEGRATION TEST') {
			steps { 
				echo "INTEGRATION TEST"
			} 
		}
	}
	post{
		always {
			echo "I am awesome, I run always"
		}
		success {
			echo "Successful"
		}
		failure {
			echo "Failed"
		}
	}
}
