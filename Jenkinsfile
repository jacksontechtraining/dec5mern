pipeline{
    agent any
    stages{
   
        stage('checking node availability'){
            steps{
                bat 'node --version'
            }
        }
    
   
        stage('checking npm availability'){
            steps{
                bat 'npm --version'
            }
        }
    
   
        stage('git checkout from VC'){
            steps{
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/jacksontechtraining/dec5mern.git']])
            }
        }
    
   
        stage('installing dependencies'){
            steps{
                bat 'npm i'
            }
        }
    
   
        stage('running test case'){
            steps{
                bat 'npm i'
            }
        }
    
   
        stage('clean build'){
            steps{
                bat 'del node_modules'
            }
        }
    }
}