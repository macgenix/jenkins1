pipeline{
    agent any

    stages{
        stage('Build'){
            steps{
                echo 'mvn clean package'
            }
        }
    }

    post{
        success {
            emailext to: 'macgenix@gmail.com', body: 'notification jenkins', subject: 'notif jenkins'
        }
    }
}