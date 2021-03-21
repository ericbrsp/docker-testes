pipeline {

  agent any

    stages {
    stage('Cloning Git') {
      steps {
        git([url: 'https://github.com/ericbrsp/docker-testes.git')

      }
    }
  

    stage('Building image') {
      steps{
        script {
          sh docker build -f dockerfile-front + ":$BUILD_NUMBER" .
        }
      }
    }
  }
}
}