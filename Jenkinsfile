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
            emailtext to: 'macgenix@gmail.com', body: 'notification jenkins', subject: 'notif jenkins'
        }
    }
}