pipeline {
	agent docker{image {maven:3.9.9}}

	stages {
		stage('Build') 
		{
			steps {
				sh 'mvn --version'
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
