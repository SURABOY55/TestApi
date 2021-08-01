pipeline {
    agent {
        docker {
            image "maven:3.6.0-jdk-8"
            label "docker"
        }
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
