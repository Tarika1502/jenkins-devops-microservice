pipeline {
	agent any
	environment {
		mavenHome = tool 'myMaven'
		dockerHome =tool 'myDocker'
		PATH = "$mavenHome/bin:$dockerHome/bin:$PATH"
	}

	stages {
		stage('Build') 
		{
			steps {
				sh 'mvn --version'
				sh 'docker version'
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
