pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                timeout(time: 1, unit: 'MINUTES') {
                    retry(5) {
                        sh 'ping 8.8.8.8'
                    }
                }
            }
        }
    }
}
