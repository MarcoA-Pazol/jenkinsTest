pipeline {
    agent any
    tools {
        maven 'apache-maven-3.9.6'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn package'
                sh 'java /src/main/java/com/mycompany/app/App.java'
            }
        }
    }
}
