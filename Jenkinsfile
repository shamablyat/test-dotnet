pipeline {
    agent any

    stages {
        stage('Build') {
            when {
                branch 'master'
            }
            steps {
                echo "Building..."
            }
        }
        stage('Deliver') {
            when {
                branch 'main'
            }
            steps {
                echo 'Deliver....'

            }
        }
    }
}

pipeline {
    agent any
    stages {
        stage('Build') {
            when {
                environment name: 'BUILD_ENV', value: 'main' // Execute this stage only if BUILD_ENV is set to 'dev'
            }
            steps {
                echo "hellooooooo from main"
            }
        }
        stage('Test') {
            when {
                environment name: 'BUILD_ENV', value: 'master' // Execute this stage only if BUILD_ENV is set to 'dev'
            }
            steps {
                echo "hellooooooo from master"
            }
        }
    }
}





