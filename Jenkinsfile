pipeline {
    agent any
    stages {
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
