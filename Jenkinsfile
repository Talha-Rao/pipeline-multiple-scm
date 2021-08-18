pipeline {
    agent any
    stages {
        stage('Node') {
            agent {
                docker {
                    image 'node:14-alpine'
                    echo "docker image"
                    

                }
            }
            steps {
                sh 'echo "Talha Rao"'
                sh 'node --version'
                
            }
        }
        stage('Maven') {
            agent {
                docker {
                    image 'maven:3.8.1-adoptopenjdk-11'
                }
            }
            steps {
                sh 'echo "Talha Rao"'
                sh 'mvn --version'
                
            }
        }
    }
}
