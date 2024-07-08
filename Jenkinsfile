pipeline {
	// agent any
	agent {docker {image 'maven:3.9.8'}}
	stages{
		stage('Build'){
			steps{
				sh "mvn --version"
				echo 'Building the project'
			}
		}
		stage('Test'){
			steps{
				echo 'Testing the project'
			}
		}
		stage('Deploy'){
			steps{
				echo 'Deploying the project'
			}
		}
	}
	post{
		always{
			echo 'This will always run'
		}
		success{
			echo 'This will run only if the pipeline is successful'
		}
		failure{
			echo 'This will run only if the pipeline is failed'
		}
	}
}
