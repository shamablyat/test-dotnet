// pipeline {
//     agent any

//     stages {
//         stage('Build') {
//             when {
//                 branch 'main'
//             }
//             steps {
//                 echo "Building..."
//                 sh '''
//                 docker build -t tajbaevsh/dotnet .
//                 '''
//             }
//         }
//         stage('Deliver') {
//             when {
//                 branch 'main'
//             }
//             steps {
//                 echo 'Deliver....'
//                 sh '''
//                 docker push tajbaevsh/dotnet:latest
//                 '''
//             }
//         }
//     }
// }

// pipeline {
//     agent any

//     stages {
//         stage('Build') {
//             steps {
//                 script {
//                     if(env.BRANCH_NAME == 'master') {
//                         sh '''
//                         echo "hello from master"
//                         '''
//                     }
//                 }
//             }
//         }
//         stage('deviler') {
//             steps {
//                 script {
//                     if(env.BRANCH_NAME == 'main') {
//                         sh '''
//                         echo "hello from main"
//                         '''
//                     }
//                 }
//             }
//         }
//     }
// }






pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Your build steps here
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                // Your test steps here
                echo 'Testing...'
            }
        }
    }

    post {
        success {
            // Execute this block of code only when code is pushed to the 'master' branch
            when {
                branch 'master'
            }
            steps {
                script {
                    // Run specific script for 'master' branch
                    echo "hello from master"
                }
            }
        }
    }
}

