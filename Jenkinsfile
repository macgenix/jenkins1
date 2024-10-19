pipeline{
    agent any

    stages{
        stage('Build'){
            failFast true
            parallel{
                stage('Build frontend'){
                    steps {
                        echo "Build"
                    }
                }

                stage('Build backend'){
                    steps {
                        echo "Build"
                    }
                }
            }
        }

        stage('Deploy PROD'){
            steps {
                echo "Deployement en production"
            }
        }
    }
}