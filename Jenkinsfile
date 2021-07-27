pipeline {
    
    agent any  
 
    stages {
 
        stage('Init'){
            steps {
                echo 'Init'
                echo '******************************'
                
                git branch: 'main', url: 'https://github.com/Base2526/node-docker-good-defaults.git'
            }
        }
 
        stage('Yarn Install') {
            steps {
                echo 'Yarn Install'
                echo '******************************'
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
