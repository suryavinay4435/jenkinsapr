pipeline {
    agent any

    tools {
	maven 'apache-maven-3.9.6'
      
    }

    stages {
        stage('code clone') {
            steps {
			git branch: 'main', credentialsId: 'Git', url: 'https://github.com/suryavinay4435/jenkins1.git'
			
                
            }
            }
			stage('code clean') {
            steps {
			sh 'mvn clean'
                
            }
            }
			stage('code validate') {
            steps {
			sh 'mvn validate'
                
            }
            }
			stage('code compile') {
            steps {
			sh 'mvn compile'
                
            }
            }
			stage('code test') {
            steps {
			sh 'mvn test'
                
            }
            }
			stage('code package') {
            steps {
			sh 'mvn package'
                
            }
            }
         }
      }