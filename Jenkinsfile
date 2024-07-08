pipeline {
	agent any
	stages{
		stage('Build'){
			steps{
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
