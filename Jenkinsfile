pipeline {
    agent any
    tools {
        maven 'apache-maven-3.0.6'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn --version'
            }
        }
    }
}
