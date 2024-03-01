pipeline {
    agent any
    stages {
        stage('Build') {
            when {
                not {
                    branch 'master'
                }
            }
            steps {
                echo "Building...."
            }
        }
        
        stage('Deliver') {
            when {
                not {
                    branch 'main'
                }
            }
            steps {
                echo 'Deliver.....'

            }
        }
    }

}





