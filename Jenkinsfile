pipeline {

    agent any



    stages {

        stage ('Compile Stage') {



            steps {

                withMaven(maven : 'maven_3_6_1') {

                   bat label: '', script: 'mvn compile'

                }

            }

        }



        stage ('Testing Stage') {



            steps {

                withMaven(maven : 'maven_3_6_1') {

                    bat label: '', script: 'mvn test'

                }

            }

        }





        stage ('Deployment Stage') {

            steps {

                withMaven(maven : 'maven_3_6_1') {

                    bat label: '', script: 'mvn deploy'

                }

            }

        }

    }

}