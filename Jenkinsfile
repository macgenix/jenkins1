pipeline{
    agent any

    tools{
        gradle 'gradle8.11'
        nodejs 'node23'
    }

    stages{
        stage('Build'){
            steps{
                sh 'gradle -v'
                sh 'node -v'
            }
        }
    }
}