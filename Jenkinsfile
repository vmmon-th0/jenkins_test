pipeline {
    agent any
    stages {

        stage('Deploy - Staging') {
            steps {
                sh 'echo 41'
                sh 'echo 42'
            }
        }

        stage('Sanity check') {
            steps {
                input "Does the staging environment look ok?"
            }
        }

        stage('Deploy - Production') {
            steps {
                sh 'prod env'
            }
        }
    }
}
