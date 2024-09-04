pipeline {
    agent any
    stages {
        stage('Exchange') {
            steps {
                sh 'mvn clean deploy' 
            }
        }
        stage('Runtime') {
            steps {
                sh 'mvn clean deploy -DmuleDeploy' 
            }
        }
    }
}
