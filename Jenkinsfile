pipeline {
    agent { label 'LongPT37' }
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
