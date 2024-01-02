pipeline {
    agent any
    stages {
        stage('Test') { 
            steps {
                withMaven() {
                    sh 'mvn package'
                }
                sh 'java -jar target/*.jar'
            }
        }
    }
}
