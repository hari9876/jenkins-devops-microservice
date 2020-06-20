pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				echo 'build'
			}
		}	
		stage('Test') {
			steps {
				echo 'Test'
			}
		}
		stage('Integration test') {
			steps {
				echo 'Integration test'
			}
		}
	}
	post{
		always {
			echo "I am awesome"
		}
		success {
			echo "I am successful"
		}
		failure {
			echo "I failed"
		}
	}
}
