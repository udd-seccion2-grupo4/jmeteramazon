pipeline {
    agent any
    stages {
        stage('Clean') {
            steps {
                script {
                        bat  "./mvnw clean"           
                }
            }
        }

        stage('Compile') {
            steps {
                script {
                        bat  "./mvnw compile -e"           
                }
            }
        }

        stage('Test') {
            steps {
                 script {
                    bat  "./mvnw verify -Pperformance"           
                }
            }
        }
    }
}
