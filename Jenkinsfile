pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                retry(3) {
                    sh 'gcc test1.c -o test1'
                }
            }
        }
        stage('Test') {
            steps {
                sh './test1'
                sh 'python hw.py'
            }
        }
    }
}
