pipeline{
    agent any


    stages{
        stage('Build'){
            steps {
                echo "Build"
            }
        }

        stage('Deploy PROD'){
            input{
                message "Voulez-vous deployer en PROD ?"
                ok 'deploy !'
                submitter 'admin, devops'
                submitParameter 'USER_SUBMIT'
                parameters{
                    string(name: 'VERSION', defaultValue:'latest', description: 'La version deployée')
                }
            }

            steps {
                echo "USER : ${USER_SUBMIT}"
                echo "VERSION : ${VERSION}"
                echo "Deployement en production"
            }
        }
    }
}