pipeline {
	//agent { docker {image 'maven:3.6.3'} }
	agent any
	environment{
		dockerHome=tool 'haridocker'
		mavenhome=tool 'Harimaven'
		PATH="$PATH:$dockerhome/bin:$mavenhome/bin"
	}
	stages {
		stage('Build') {
			steps {
				sh 'mvn --version'
				sh 'docker version'
			//	echo 'build'
			//	echo '$PATH'
			//	echo "build number - $env.BUILD_NUMBER"
			//	echo "Job Name - $env.JOB_NAME"
			//	echo "Build URL - $env.BUILD_URL"				
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
