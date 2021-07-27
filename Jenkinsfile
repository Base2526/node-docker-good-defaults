pipeline {
    
     environment {
       // registry = “bkshashi9/webapp”
       // registryCredential = ‘dockerhub’
       dockerImage = ''
         
         registry = "naistangz/docker_automation"
     }
    
    agent any  
 
    stages {
 
        stage('Cloning Git'){
            steps {
                echo 'Cloning Git'
                echo '******************************'
                
                git branch: 'main', url: 'https://github.com/Base2526/node-docker-good-defaults.git'
            }
        }
 
        stage('Building Docker Image') {
            steps {
                echo 'Building Docker Image'
                echo '******************************'
                
                // dockerImage = docker.build "yenigul/hacicenkins"
                script {
                    // dockerImage = docker.build "yenigul/hacicenkins"
                    // dockerImage = docker.build "yenigul/hacicenkins"
                    
                    dockerImage = docker.build registry + ":$BUILD_NUMBER"
                }
            }
        }
 
        stage('Yarn Build') {
            steps {
                echo 'Yarn Build'
                echo '******************************'
            }
        }
  
        stage('Deploy') {
            steps{
                echo 'Deploy'
                echo '******************************'
            }
        }
    }
}
