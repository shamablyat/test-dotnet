pipeline {
    agent any
    stages {
        stage('Preparation') {
            when {
                env.BRANCH_NAME "master"
            }
            steps {
                checkout scm
            }
            
        }
        stage('Who am i?') {
            when {
                env.BRANCH_NAME "master"
            }
            steps {
                echo "This job was triggered by a Git push to branch: ${env.BRANCH_NAME}"
            }
        }
    }

}