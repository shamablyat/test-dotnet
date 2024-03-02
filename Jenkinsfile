pipeline {
    agent any
    stages {
        stage('master') {
            when {
                branch "master"
            }
            steps {
                echo "master"
            }
            
        }
        stage('main') {
            when {
                branch "main"
            }
            steps {
                echo "main."
            }
        }
    }

}