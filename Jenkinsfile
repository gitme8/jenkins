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

// pipeline {
//     agent any
//     environment {
//         URL1 = "google.com"
//         SSH = credentials("CENTOS")
//         SSH1 = credentials("new-secret-key1")
//     }
//     stages {
//         stage('ONE') {
//             steps{
//                 sh 'echo ${URL1}'
//                 echo SSH
//                 sh 'env'
//                 sh 'echo ${SSH1} | base64'
//             }
//         }
//     }
// }

// pipeline {
//     agent any
//     parameters {
//         string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
//
//         text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')
//
//         booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
//
//         choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
//
//         password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter the password')
//     }
//     stages {
//         stage('Example') {
//             steps {
//                 echo "Hello ${params.PERSON}"
//
//                 echo "Biography: ${params.BIOGRAPHY}"
//
//                 echo "Toggle: ${params.TOGGLE}"
//
//                 echo "Choice: ${params.CHOICE}"
//
//                 echo "Password: ${params.PASSWORD}"
//             }
//         }
//     }
// }

// pipeline {
//     agent any
//     tools {
//        maven 'maven-3.8.6'
//     }
//     stages {
//         stage('Maven') {
//             steps {
//                 sh 'mvn --version'
//             }
//         }
//     }
// }

// pipeline {
//     agent any
//     stages {
//         stage('Example') {
//             input {
//                 message "Should we continue?"
//                 ok "Yes, we should."
//                 submitter "alice,bob"
//                 parameters {
//                     string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
//                 }
//             }
//             steps {
//                 echo "Hello, ${PERSON}, nice to meet you."
//             }
//         }
//     }
// }

// pipeline {
//     agent any
//     parameters {
//         choice(name: 'ENV', choices: ['DEV', 'PROD'], description: 'Pick Environment')
//     }
//     stages {
//         stage('DEV') {
//             when {
//                environment name: 'ENV', value: 'DEV'
//             }
//             steps {
//                 echo "DEV"
//             }
//         }
//          stage('PROD') {
//             when {
//                 environment name: 'ENV', value: 'PROD'
//             }
//             steps {
//                  echo "PROD"
//
//             }
//         }
//     }
// }

// pipeline {
//     agent any
//     stages {
//
//         stage('One-Sequential') {
//             steps {
//                 sh 'sleep 40'
//             }
//         }
//
//         stage('Two-Parallel') {
//             parallel {
//                 stage('Two1') {
//                     steps {
//                         sh 'sleep 50'
//                     }
//                 }
//
//                 stage('Two2') {
//                     steps {
//                         sh 'sleep 70'
//                     }
//                 }
//             }
//         }
//     }
// }