pipeline {
    agent any
    tools {
        maven 'apache-maven-3.9.6'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'java -jar /src/main/com/mycompany/app/App.java'
            }
        }
    }
}
