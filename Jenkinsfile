pipeline {
    agent any
    when{
        branch : "master"

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
                    echo 'Deliver....'

                }
            }
        }
    }
}





