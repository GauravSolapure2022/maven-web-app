pipeline {  

    agent any
        
    tools{
        maven "Maven-3.9.0"
    }
    stages {
        stage('Clone') {
            steps {
               git 'maven-web-app.git'
            }
        }
        stage('Build') {
            steps {
               sh 'mvn clean package'
            }
        }
    }
}
