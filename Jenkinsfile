pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/HarshitaRaotole/simplejavaapp.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean install'  // Use bat instead of sh
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'  // Use bat instead of sh
            }
        }

        stage('Deploy') {
            steps {
                bat 'mvn deploy'  // Use bat instead of sh
            }
        }
    }
}
