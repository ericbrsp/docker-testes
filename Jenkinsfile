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
                script{ 
                    docker.build("teste-1")
                }
            }
        }
        stage('Deploy') { 
            steps {
             echo "deploy" 
            }
        }
    }
}