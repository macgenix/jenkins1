pipeline{
    agent any

    parameters{
        booleanParam(name: 'DEPLOY_TO', defaultValue: false,  description: 'Production ?')

    }

    stages{
        stage('Build'){
            steps {
                echo "Build"
            }
        }

        stage('Deploy PROD'){
            when{
                allOf{
                    branch 'main'
                    equals  expected: true, actual: params.DEPLOY_TO

                }
            }

            steps {
                echo "Deployement en production"
            }
        }
    }
}