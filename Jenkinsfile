pipeline {
    agent any
    stages {
        stage('Test') { 
            steps {
                withMaven( maven: 'MVN' ) {
                    sh 'mvn clean verify'
                    sh 'mvn package'
                }
                sh 'java -jar target/*.jar'
            }
        }
    }
}
