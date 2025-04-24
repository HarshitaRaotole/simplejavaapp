pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building the application'
                bat 'mvn clean install'  // Adjust this to your build tool (e.g., Maven or Gradle)
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests'
                bat 'mvn test'  // Adjust this to run your tests
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application'
                // Add deployment steps here
            }
        }
    }
}
