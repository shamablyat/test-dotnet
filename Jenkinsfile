pipeline {
    agent any

    stages {
        stage('Build') {
            when {
                branch 'master'
            }
            steps {
                echo "Building..."
                sh '''
                echo "hello world from master"
                '''
            }
        }
        stage('Deliver') {
            when {
                branch 'main'
            }
            steps {
                echo 'Deliver....'
                sh '''
                echo "hello world from main"
                '''
            }
        }
    }
}






