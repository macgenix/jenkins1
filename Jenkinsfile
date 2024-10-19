pipeline{
    agent any

    stages{
        stage('Build'){
            steps{
                sh 'echo Building > word.txt'
                archiveArtifacts(artifacts: '*.txt')
            }
        }
    }
}