pipeline {
    agent any
    stages {
        stage('master.') {
            when {
                branch "master"
            }
            steps {
                sh '''
                rm -rf test-dotnet
                git clone https://github.com/shamablyat/test-dotnet/
                cd test-dotnet 
                ls
                pwd
                sudo docker compose up --build -d
                docker ps
                '''
            }
        }
        stage('main') {
            when {
                branch "main"
            }
            steps {
                sh '''
                rm -rf test-dotnet
                git clone https://github.com/shamablyat/test-dotnet/
                cd test-dotnet 
                ls
                pwd
                dotnet run --launch-profile https
                '''
            }
        }
    }
}