pipeline {
    agent any
    stages {
        stage('Build') {
            when {
            
                branch "main"
        
            }
            steps {
                echo "Building..."
            }
        }
        stage('Deliver') {
            when {
                branch "master"
                
            }
            steps {
                echo 'Deliver.....'

            }
        }
    }

}





