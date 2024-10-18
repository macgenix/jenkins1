pipeline{
    agent any
    
    options{
        timeout(time:1, unit:"HOURS")
    }

    parameters{
        string(name: 'NAME', defaultValue: 'Jenkins Param string',  description: 'Jenkins Param string')
        text(name: 'TEXT', defaultValue: 'Jenkins Param text',  description: 'Jenkins Param text')
        booleanParam(name: 'TOOGLE', defaulValue: true,  description: 'Jenkins Param boolean')
        choise(name: 'CHOICE', choices:['un', 'deux', 'trois'],  description: 'Jenkins Param text')
        password(name: 'PASSWORD', description: 'Jenkins Param un mot de passe')
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

        stage('Tests'){
            steps{
                echo  "NAME: ${NAME}"
                echo  "TEXT: ${TEXT}"
                echo  "TOOGLE: ${TOOGLE}"
                echo  "CHOICE: ${CHOICE}"
                echo  "PASSWORD: ${PASSWORD}"
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