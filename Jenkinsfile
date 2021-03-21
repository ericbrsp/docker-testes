pipeline {
  environment {

  }
  
  agent any

    stages {
    stage('Cloning Git') {
      steps {
        git([url: 'https://github.com/ericbrsp/docker-testes.gitt', branch: 'master', credentialsId: 'ericbrs['])

      }
    }
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
