pipeline{
    agent any


    stages{
        stage('Build and test'){
            matrix{
                axes{
                    axis{
                        name 'OS'
                        values 'Windows', 'Linux'
                    }

                    axis{
                        name 'BROWSER'
                        values 'Chrome', 'Firefox'
                    }
                }

                stages{
                    stage('Build'){
                        steps{
                            echo "Construire pour  ${OS} et ${BROWSER}"

                        }
                    }

                    stage('Tests'){
                        steps{
                            echo "Test  pour  ${OS} et ${BROWSER}"

                        }
                    }
                }
            }
        }

        stage('Deploy PROD'){
            steps {
                echo "Deployement en production"
            }
        }
    }
}