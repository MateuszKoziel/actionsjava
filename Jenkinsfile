pipeline {
    agent { docker { image 'maven:3.8.8-eclipse-temurin-21' } }
    stages {
        stage('Example Build') {
            steps {
                echo 'Building the Java project'
                sh 'mvn clean package'
            }
        }
        stage('Example Test') {
            steps {
                echo 'Running tests'
                sh 'mvn test'
            }
        }
    }
}