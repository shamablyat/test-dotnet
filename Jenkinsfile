pipeline {
    agent any
    stages {
        
        stage('Preparation') {
            steps {
                checkout scm
            }
            
        }
        stage('Who am i?') {
            steps {
                echo "This job was triggered by a Git push to branch: ${env.BRANCH_NAME}"
            }
        }
    }

}