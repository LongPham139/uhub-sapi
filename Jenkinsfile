pipeline {
    agent { label 'Idle'}
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
