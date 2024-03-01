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

pipeline {
    agent any

    stages {
        stage('Build') {
            when {
                branch 'master'
            }
            steps {
                echo "Building..."
                sh '''
                echo "hello from master"
                '''
            }
        }
    }
    stage('Deliver') {
        when {
            branch 'main'
        }
        steps {
            echo 'Deliver....'
            sh '''
            echo "hello from main"
            '''
        }
    }
}