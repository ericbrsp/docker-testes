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
                    echo "Olá Deploy" 
            }
        }
        stage('Deploy') { 
            steps {
             echo "deploy" 
            }
        }
    }
}