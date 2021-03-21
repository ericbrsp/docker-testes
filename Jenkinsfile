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
            sh 'docker build -f dockerfile-front . '
            }
        }
        stage('Deploy') { 
            steps {
             echo "deploy" 
            }
        }
    }
}