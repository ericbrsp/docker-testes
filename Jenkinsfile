pipeline {
    agent any 
    stages {
        stage('Clonando o GIT') { 
            steps {
            git 'https://github.com/ericbrsp/docker-testes.git'    
            }
        }
        stage('Building image') { 
            steps {
       //     echo "teste"    //
            docker.build("my-image:${env.BUILD_ID}")
            }
        }
        stage('Deploy') { 
            steps {
             echo "deploy" 
            }
        }
    }
}