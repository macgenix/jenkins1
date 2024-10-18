pipeline{
    agent any


    stages{
        stage('Build'){
            steps {
                echo "Build"
            }
        }

        stage('Deploy PROD'){
            when{
                branch 'main'
            }

            steps {
                echo "Deployement en production"
            }
        }
    }
}