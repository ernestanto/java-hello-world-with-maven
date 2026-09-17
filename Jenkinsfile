pipeline {
    agent any

    tools {
        maven 'Maven-3.8.4'
    }

    stages {
       stage('Build') {
    steps {
        sh 'echo "PATH=$PATH"'
        sh 'echo "MAVEN_HOME=$MAVEN_HOME"'
        sh 'ls -la /usr/share/maven/bin/'
        sh 'ls -la "$MAVEN_HOME/bin/mvn" || true'
    }
}
    }
}