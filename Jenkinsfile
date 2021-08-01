pipeline {
    agent any
    stages {
        stage('Build Maven'){
            steps {
                sh "mvn -version"
                sh "mvn clean install"
            }
        }
    }  
}
