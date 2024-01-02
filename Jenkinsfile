pipeline {
    agent any
    stages {
        stage('Test') { 
            steps {
                withMaven( mavenLocalRepo: '.repository' ) {
                    sh 'mvn package'
                }
                sh 'java -jar target/*.jar'
            }
        }
    }
}
