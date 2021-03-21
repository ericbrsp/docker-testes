pipeline {
  environment {

  }
  
  agent any

    stages {
    stage('Cloning Git') {
      steps {
        git([url: 'https://github.com/ericbrsp/docker-testes.gitt', branch: 'master', credentialsId: '25ca1b5b-0371-4a2f-b099-3c77436e49f4'])

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
}