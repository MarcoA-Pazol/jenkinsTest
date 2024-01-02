pipeline {
    agent any
    stages {
        stage('Test') { 
            steps {
                withMaven {
                    sh 'mvn clean package'
                }
                sh 'java -jar target/*.jar'
            }
        }
    }
}
