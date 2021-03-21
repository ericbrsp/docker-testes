pipeline {

  agent any

    stages {
    stage('Cloning Git') {
      steps {
        git([url: 'https://github.com/ericbrsp/docker-testes.git', branch: 'main', credentialsId: '25ca1b5b-0371-4a2f-b099-3c77436e49f4'])

      }
    }
  }

    stage('Building image') {
      steps{
        script {
          docker build -f dockerfile-front + ":$BUILD_NUMBER" .
        }
      }
    }
  

}