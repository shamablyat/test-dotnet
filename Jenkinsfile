pipeline {
    agent any
    stages {
        stage('Build') {
            when {
                not {
                    branch "master"
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





