pipeline {
	agent any
	stages {
		stage('Build') 
		{
			echo "Build"
		}
		stage('Test') {
			echo "Test"
		}
		stage('Integration Test') {
			echo "Integration Test"
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
