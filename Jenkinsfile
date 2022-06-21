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
        
        }
    }
