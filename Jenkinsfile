pipeline {
    agent any

    tools {
        maven "3.8.1"
    }
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
    post{
        always {
            cleanWs()
        }
    }  
}
