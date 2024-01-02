pipeline {
    agent any
    stages {
        stage('Test') { 
            steps {
                withMaven {
                    sh 'mvn clean verify 
                    sh 'mvn package'
                }
                sh 'java -jar target/*.jar'
            }
        }
    }
}
