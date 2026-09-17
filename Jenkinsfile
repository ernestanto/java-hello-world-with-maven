pipeline {
    agent any

    stages {
      stage('Build') {
    steps {
        sh '''
            echo "=== SHELL PID ==="
            echo $$

            echo "=== PARENT PID ==="
            ps -o pid,ppid,user,cmd -p $$

            echo "=== PROCESS ROOT ==="
            readlink /proc/$$/root

            echo "=== MOUNTS ==="
            cat /proc/$$/mountinfo | head -20
        '''
    }
}
    }
}