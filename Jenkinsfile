pipeline {
    agent any

    stages {
       stage('Build') {
    steps {
        sh '''
            echo "=== ROOT ==="
            ls -ld /
            echo "=== USR ==="
            ls -ld /usr
            echo "=== USR SHARE ==="
            ls -ld /usr/share
            echo "=== MAVEN ==="
            ls -ld /usr/share/maven || true
            echo "=== MOUNT INFO ==="
            grep -E ' /usr | /usr/share|/var/lib/jenkins' /proc/self/mountinfo || true
        '''
    }
}
    }
}