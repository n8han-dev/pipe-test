pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                retry(3) {
                    sh "ls"
                    // sh 'chmod +x test3.sh'
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
