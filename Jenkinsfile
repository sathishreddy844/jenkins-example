pipeline {
    agent {label 'linux-node'}

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
                maven 'maven3.8.5'
            }

            steps {
                    sh 'mvn test'
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
