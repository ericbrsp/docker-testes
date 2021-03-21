pipeline {
  environment {
    #registry = "docker_hub_account/repository_name"
    #registryCredential = 'dockerhub'
  }
  
  agent any
  
  stages {
    stage('Building image') {
      steps{
        script {
          docker.build docker-front + ":$BUILD_NUMBER"
        }
      }
    }
  }
}
