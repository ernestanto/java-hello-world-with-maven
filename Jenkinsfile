pipeline {
    agent any

    stages {
       stage('Build') {
    steps {
        sh '''
            echo "USER:"
            whoami

            echo "CURRENT DIRECTORY:"
            pwd

            echo "MAVEN:"
            ls -ld /usr/share/maven
            ls -ld /usr/share/maven/bin
            ls -l /usr/share/maven/bin/mvn

            echo "PROCESS:"
            ps -ef | grep '[s]h'
        '''
    }
}
    }
}