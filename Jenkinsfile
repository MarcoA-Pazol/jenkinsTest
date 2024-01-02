pipeline {
    agent any
    stages {
        stage('Test') { 
            steps {
                withMaven( maven: 'MVN' ) {
                    sh 'mvn clean verify'
                }
            }
        }
        stage('Build') {
            tools {
                maven 'MVN'
            }
            steps {
                sh 'mvn package'
                sh 'java -jar target/*.jar'
            }
        }
    }
}
