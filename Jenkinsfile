pipeline {
    agent any
    stages {
        stage('Build') {
            when {
                not {
                    branch "main"
                }
            }
            steps {
                echo "Building..."
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver.....'

            }
        }
    }

}





