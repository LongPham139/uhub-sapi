pipeline {
    agent any
    tools {
        maven 'Maven 3.8.1' // Ensure this matches the name of your Maven installation in Jenkins
    }
    stages {
        stage('Clean') {
            steps {
                bat 'mvn clean install -X' 
            }
        }
        stage('Exchange') {
            steps {
                bat 'mvn clean deploy -X' 
            }
        }
        stage('Runtime') {
            steps {
                bat 'mvn clean deploy -DmuleDeploy -X' 
            }
        }
    }
}
