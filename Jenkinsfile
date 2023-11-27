pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                withMaven(maven : 'maven_4_0_0') {
                    sh 'mvn clean compile'
                }
            }
        }
        stage('Test') {
            steps {
                withMaven(maven : 'maven_4_0_0') {
                    sh 'mvn test'
                }
            }
        }
    }
}