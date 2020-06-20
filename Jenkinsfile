pipeline {
	agent { docker {image 'maven:3.6.3'} }
	//agent any
	stages {
		stage('Build') {
			steps {
				sh 'mvn --version'
				sh 'whoami'
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
