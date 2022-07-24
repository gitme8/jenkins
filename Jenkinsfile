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
    agent none
    environment {
        URL = "google.com"
    }
    stages {
        stage('ONE') {
            steps{
                sh 'echo ${URL}'
                echo URL
            }
        }
    }
}