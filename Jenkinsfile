pipeline {

  agent any

    stages {
    stage('Cloning Git') {
      steps {
        git([url: 'https://github.com/ericbrsp/docker-testes.gitt', branch: 'main', credentialsId: '25ca1b5b-0371-4a2f-b099-3c77436e49f4'])

      }
    }

    stage('Building image') {
      steps{
        script {
          docker.build docker-front + ":$BUILD_NUMBER"
        }
      }
    }
  
}
}