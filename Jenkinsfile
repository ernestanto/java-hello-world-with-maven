pipeline {
    agent any

    stages {

        stage('Build') {
    steps {
        sh 'echo "PATH=$PATH"'
        sh 'whoami'
        sh 'command -v mvn || true'
        sh 'ls -l /usr/bin/mvn'
        sh '/usr/bin/mvn -version'
    }
}

    }
}