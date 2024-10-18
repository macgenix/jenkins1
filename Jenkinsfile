pipeline{
    agent any
    
    options{
        timeout(time:1, unit:"HOURS")
    }

    parameters{
        string(name: 'PERSONNE', defaultValue: 'M. Jenkins', description: 'À qui devrais-je dire bonjour ?')
        text(name: 'BIOGRAPHIE', defaultValue: '', description: 'Entrez des informations sur la personne')
        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Activez cette valeur')
        choice(name: 'CHOIX', choices: ['Un', 'Deux', 'Trois'], description: 'Faites un choix')
        password(name: 'MOT_DE_PASSE', defaultValue: 'SECRET', description: 'Entrez un mot de passe')
    }

    stages{
        stage('Build'){
            steps {
                echo "Bonjour ${PERSONNE}"
                echo "Biographie : ${BIOGRAPHIE}"
                echo "Toggle : ${TOGGLE}"
                echo "Choix : ${CHOIX}"
                echo "Mot de passe : ${MOT_DE_PASSE}"
            }
        }

        stage('Tests'){
            steps {
                echo "Bonjour ${PERSONNE}"
                echo "Biographie : ${BIOGRAPHIE}"
                echo "Toggle : ${TOGGLE}"
                echo "Choix : ${CHOIX}"
                echo "Mot de passe : ${MOT_DE_PASSE}"
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