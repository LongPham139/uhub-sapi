pipeline {
    agent any
    tools {
        maven 'Maven 3.8.1' // Ensure this matches the name of your Maven installation in Jenkins
    }
    stages {
        stage('Clean') {
            steps {
                bat 'mvn clean install' 
            }
        }
        stage('Exchange') {
            steps {
                bat 'mvn clean deploy' 
            }
        }
        stage('Runtime') {
            steps {
                bat 'mvn clean deploy -DmuleDeploy' 
            }
        }
    }
}
