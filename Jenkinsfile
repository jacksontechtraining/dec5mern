pipeline{
    agent any
    stages{
        stage('checking node availability'){
            steps{
                bat 'node --version'
            }
        }
    }
    stages{
        stage('checking npm availability'){
            steps{
                bat 'npm --version'
            }
        }
    }
    stages{
        stage('git checkout from VC'){
            steps{
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/jacksontechtraining/dec5mern.git']])
            }
        }
    }
    stages{
        stage('installing dependencies'){
            steps{
                bat 'npm i'
            }
        }
    }
    stages{
        stage('running test case'){
            steps{
                bat 'npm i'
            }
        }
    }
    stages{
        stage('clean build'){
            steps{
                bat 'del node_modules'
            }
        }
    }
}