pipeline {
    agent any
    stages{
        stage('Build'){
            steps{
                bat 'mvn clean package -X'
                bat "docker build . -t tomcatwebapp:${env.BUILD_ID}"
            }
        }
    }
}