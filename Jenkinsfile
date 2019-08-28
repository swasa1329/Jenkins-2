pipeline {

    agent any



    stages {

        stage ('Compile Stage') {



            steps {

                withMaven(maven : 'maven_3_6_1') {

                    'mvn clean compile'

                }

            }

        }



        stage ('Testing Stage') {



            steps {

                withMaven(maven : 'maven_3_6_1') {

                    'mvn test'

                }

            }

        }





        stage ('Deployment Stage') {

            steps {

                withMaven(maven : 'maven_3_6_1') {

                    'mvn deploy'

                }

            }

        }

    }

}