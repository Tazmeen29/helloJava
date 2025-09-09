pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
                git branch: 'main', credentialsId: '5e4b73d7-59b1-4bdb-87d4-c315a954cc54', url: 'https://github.com/Tazmeen29/helloJava.git'
            }
        }
        
        stage('Compile') {
            steps {
                bat 'javac HelloJava.java' 
            }
        }
    
        stage('Run') {
            steps {
                bat 'java HelloJava'
            }
        }
    }
}
