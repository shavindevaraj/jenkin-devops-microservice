pipeline {
	agent {docker{image 'maven:3.6.3'}}
	stages{
		stage('Build') {
			steps{
			sh 'mvn --version'
			echo "Build"
			}
		}
		stage('Test') {
			steps{
			echo "Test"
			}
		}
		stage('Integration Test') {
			steps{
			echo "Integration Test"
			}
		}
}
post{
	always{
		echo "I'm awesome.I run always"
	}
	success{
		echo "I will run only if u succeed"
	}
	failure{
		echo "I will run only if u fail"
	}
}
}
