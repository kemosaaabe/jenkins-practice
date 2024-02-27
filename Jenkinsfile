pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'gcc -o myapp main.c'
            }
        }

        stage('Archive') {
            steps {
                archiveArtifacts artifacts: 'myapp', fingerprint: true
            }
        }
    }
}

