pipeline {
    agent any
    stages{
        stage('Git Clone'){
            steps{
                git branch: 'main', url: 'https://github.com/Midguar11/HelloWorld-Springboot-App-.git'
            }
        }
        
        stage('Maven Test'){
            steps{
                sh 'mvn test'
            }
        }
        
        stage('Maven Package'){
            steps{
                sh 'mvn package'
            }
        }
        
        stage('Maven Deploy'){
            steps{
                echo " Deploying the ar file to the server "
            }
        }
    }
}
