pipeline{
    agent any
    
    options{
        timeout(time:1, unit:"HOURS")
    }

    triggers{
        pollSCM('* * * * * *')

    }

    stages{
        stage('Build'){
            steps {
                echo "Build"
            }
        }

        stage('Tests'){
            steps {
                echo "Test"
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