pipeline {
    agent docker {
        image '3.9.6-eclipse-temurin-11'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn --version'
            }
        }
    }
}
