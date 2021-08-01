pipeline {
    agent any
    stages {
        stage('Build Maven'){
            steps {
                sh '''
                   mvn clean install
                   pwd
                   echo "end download maven"
                '''
            }
        }
    }  
}
