// Scripted pipeline
pipeline {              
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    sh """
                        echo "Building"
                    """
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    sh """
                        echo "Testing"
                    """
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    sh """
                        echo "Deploying"
                    """
                }
            }
        }
    }
}

// Declarative pipeline

// pipeline {                   
//     agent any
//     stages {
//         stage('Build') {
//             steps {
//                 echo "Building"
//             }
//         }
//         stage('Test') {
//             steps {
//                 echo "Testing"
//             }
//         }
//         stage('Deploy') {
//             steps {
//                echo "Deploying"
//             }
//         }
//     }
// }