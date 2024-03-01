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
            when {
                not {
                    branch "master"
                }
            }
            steps {
                echo 'Deliver.....'

            }
        }
    }

}





