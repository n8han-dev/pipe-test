pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh "ls"
                retry(3) {
                    sh 'chmod +x test3.sh'
                }
            }
        }
        stage('Test') {
            steps {
                sh 'echo "-------------------test 1----------------"'
                sh 'python hw.py'
                sh './test3.sh'
            }
        }
    }
}
