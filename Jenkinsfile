pipeline {
	agent any
	stages {
		stage('Clone') {
			steps {
				git branch: 'master', url: 'https://github.com/pdhoang91/jenkin.git'
			}
		}
		// stage('Build Java App') {
		// 	steps {
		// 		withDockerRegistry(credentialsId: 'docker-hub', url: 'https://index.docker.io/v1/') {
  //   				sh 'docker build -t pdhoang91/study_docker:v4'
  //   				sh 'docker push -t pdhoang91/study_docker:v4'
		// 		}
		// 	}
		// }
	}
}