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
                    echo "Olá Imagem" 
            }
        }
        stage('Deploy') { 
            steps {
             echo "deploy" 
            }
        }
    }
}