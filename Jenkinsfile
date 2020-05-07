pipeline {
    agent any
    stages {
        stage('Build'){
            steps{
                sh '/usr/local/Cellar/mvn clean package'
                sh "docker build . -t tomcatwebapp:${env.BUILD_ID}"
            }
        }
    }
}