pipeline{
    agent any
    
    options{
        timeout(time:1, unit:"HOURS")
    }

    stages{
        stage('Build'){
            
            options{
                timestamps()
            }

            steps{
                echo  'Building...'

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