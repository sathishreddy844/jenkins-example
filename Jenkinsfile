pipeline {
    agent {label 'linux-node'}

    stages {
        stage ('Clean Stage') {
            tools {
                    maven 'mvn3.8.5'
            }

            steps {
                    sh 'mvn clean'
                }
            }
        stage ('install'){
            steps{
            sh 'mvn install'
            }
        }
    }
    post {
        success {
            echo 'build is successful'
        }
        failure {
            echo 'build is failure'
        }
    }
}
