pipeline {
    agent any
    stages {
        stage('Test') { 
            steps {
                withMaven( mavenLocalRepo: '.' ) {
                    sh 'mvn package'
                }
                sh 'java -jar target/*.jar'
            }
        }
    }
}
