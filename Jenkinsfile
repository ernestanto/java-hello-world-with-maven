pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'echo "PATH=$PATH"'
                sh 'java -version'
                sh 'mvn -version'
                sh 'mvn clean package'
            }
        }
    }
}