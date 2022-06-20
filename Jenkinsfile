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
        

        stage ('compile Stage') {
            tools {
                maven 'maven3.8.5'
            }

            steps {
                    sh 'mvn compile'
                }
            }
        stage ('package') {
            tools {
                maven 'maven3.8.5'
            }
            steps {
           
                    sh 'mvn package'
                }
            }
        }
    }
