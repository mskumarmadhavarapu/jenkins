pipeline {
    agent {
        node {
            label 'ROBOSHOP'
        }
    }
    environment { 
        COURSE = 'Jenkins'
    }
    options { 
        disableConcurrentBuilds()
        timeout(time: 5, unit: 'SECONDS') 
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
                        sleep 10
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