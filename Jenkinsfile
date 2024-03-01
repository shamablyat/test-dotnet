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
        stage('Check Branch') {
            steps {
                script {
                    def branchName = env.BRANCH_NAME
                    if (branchName == 'master') {
                        echo 'Running script for master branch'
                        // Run script for master branch
                    } else if (branchName == 'main') {
                        echo 'Running script for main branch'
                        // Run script for main branch
                    } else {
                        error "Unsupported branch: ${branchName}"
                    }
                }
            }
        }
    }
}
