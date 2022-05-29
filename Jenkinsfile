pipeline {
	agent any 
	stages {
		stage ('BUILD') {
			steps { 
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
