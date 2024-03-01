pipeline {
    agent any
    when{
        branch : "master"
    }
    stages {
        stage('Build') {
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

pipeline {
    agent any
    when{
        branch : "main"
    }
    stages {
        stage('Build1') {
            steps {
                echo "Building1..."
            }
        }
        stage('Deliver1') {
            steps {
                echo 'Deliver1....'

            }
        }
    }
}



