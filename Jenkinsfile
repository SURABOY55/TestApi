pipeline {
    agent any

    tools {
        maven "MAVEN_HOME"
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
