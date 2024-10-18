pipeline{
    agent any
    
    agent{
        docker{
            image 'node:23-alpine'
        }
    }

    stages{
        stage('Build'){
            steps{
                sh 'npm -v'
            }
        }
    }

    post{
        always{
            echo 'always !'
        }

        success{
            echo 'success !'
        }
    }
}