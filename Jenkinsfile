pipeline{
    agent any

    stages{
        stage('Build'){
            sh 'echo Building > word.txt'
            archiveArtifacts(artifacts: '*.txt')
        }
    }
}