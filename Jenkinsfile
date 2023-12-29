pipeline {
    agent {
        docker {
            image '3-eclipse-temurin-17'
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn --version'
            }
        }
    }
}
