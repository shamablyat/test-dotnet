pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Building...."
                sh '''
                docker build -t tajbaevsh/dotnet .
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                docker push tajbaevsh/dotnet:latest
                '''
            }
        }
    }
}