pipeline {
	agent any
	stages {
		stage('Clone') {
			steps {
				git branch: 'main', url: 'https://github.com/pdhoang91/aws-study.git'
			}
		}
		stage('Build Docker') {
			steps {
				withDockerRegistry(credentialsId: 'docker-hub', url: 'https://index.docker.io/v1/') {
    // some block
    				sh 'docker build -t pdhoang91/study_docker:v4'
    				sh 'docker push -t pdhoang91/study_docker:v4'
				}
			}
		}
	}
}