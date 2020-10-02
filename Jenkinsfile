pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                retry(3) {
                    sh 'ls'
                }
            }
        }
        stage('Test') {
            steps {
                sh 'echo "-------------------test 1----------------"'
                sh 'python hw.py'
            }
        }
    }
}
