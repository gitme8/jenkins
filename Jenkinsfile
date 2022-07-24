// /*
// pipeline {
//     agent any
//
//     stages {
//         stage('One') {
//             steps {
//                 echo 'Hi, World'
//             }
//         }
//         stage('Two') {
//             steps {
//                 echo 'Hello, World!'
//             }
//         }
//         stage('Three') {
//             steps {
//                 echo 'Hello, World!!'
//             }
//         }
//     }
// } */

pipeline {
    agent any
    environment {
        URL1 = "google.com"
        SSH = credentials("CENTOS")
        SSH1 = credentials("common/ssh")
    }
    stages {
        stage('ONE') {
            steps{
                sh 'echo ${URL1}'
                echo SSH
                sh 'env'
                sh 'echo ${SSH1} | base64'
            }
        }
    }
}