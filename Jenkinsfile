pipeline {
    agent any

    stages {
        stage ('Clean Stage') {
            tools {
                    maven 'maven3.8.5'
            }

            steps {
                    sh 'mvn clean'
                }
            }
        

        stage ('Testing Stage') {
            tools {
                maven 'maven3.8.1'
            }

            steps {
                    sh 'mvn test'
                }
            }
        


        stage ('package') {
            tools {
                maven 'maven3.6.0'
            }
            steps {
           
                    sh 'mvn deploy'
                }
            }
        }
    }
