pipeline {
    agent any
    stages {
        stage('Test') { 
            steps {
                withMaven( maven: 'MVN' ) {
                    sh 'mvn verify'
                }
            }
        }
        stage('Clean') {
            tools {
                maven 'MVN'
            }
            steps {
                sh 'mvn clean'
            }
        }
        stage('Build') {
            agent {
                docker {
                    image 'maven:latest'
                }
            }
            steps {
                sh 'mvn package'
                sh 'java -jar target/*.jar'
            }
        }
    }
}
