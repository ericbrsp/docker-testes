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
                    docker.build("test-image", "./front")
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