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
                sh '''
                git clone https://github.com/shamablyat/test-dotnet/
                cd test-dotnet 
                ls
                pwd
                '''
            }
        }
    }
}