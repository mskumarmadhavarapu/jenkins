pipeline {              
    agent {
        node {
            label 'ROBOSHOP'
        }
    }
    environment { 
        COURSE = 'Jenkins'
    }
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
                        echo $COURSE
                    """
                }
            }
        }
    }

    // post build
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success { 
            echo 'pipeline success'

        }
        failure { 
            echo 'pipeline failure'
        }
    }
}