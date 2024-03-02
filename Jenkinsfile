pipeline {
    agent any
    stages {
        when {
            branch "master"
        }
        stage('Build') {
            steps {
                echo "Building..."
            }
        }

        stage('Deliver') {
            when {
            branch "main"
        }
            steps {
                echo 'Deliveer....'

            }
        }
    }

}





