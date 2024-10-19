pipeline{
    agent any

    tools{
        gradle 'gradle8.11'
    }

    stages{
        stage('Build'){
            steps{
                sh 'gradle -v'
            }
        }
    }
}