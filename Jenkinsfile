pipeline {
    agent any
    
    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/HarshitaRaotole/simplejavaapp.git'
            }
        }
        stage('Build') {
            steps {
                script {
                    // Assuming the Java file is SimpleJavaApp.java
                    bat 'javac SimpleJavaApp.java'
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    // Run any tests here, for example
                    bat 'java SimpleJavaApp'
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    // Deployment steps go here
                }
            }
        }
    }
}
