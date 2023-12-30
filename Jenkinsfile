pipeline {
    agent any
    tools {
        maven 'apache-maven-3.9.6'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B /src/main/com/mycompany/app/App.java'
            }
        }
    }
}
