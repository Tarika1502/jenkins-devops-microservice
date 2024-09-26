pipeline {
	agent any
	stages {
		stage('Build') 
		{
			steps {
				echo "Build"
			}
		}
		stage('Test') 
		{
			steps {
				echo "Test"
			}
		}
		stage('Integration') 
		{
			steps {
				echo "Integration test"
			}
		}
	}
	post {
		failure {
			echo "I run when build fail !!"
		}
		success {
			echo "I run when build is successful !!"
		}
		always {
			echo "I am awesome!!"
		}
	}
}
