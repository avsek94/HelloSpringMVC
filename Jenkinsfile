pipeline {
    agent any

    stages {

        stage('compile stage') {
            steps{
                withMaven(maven : 'apache-maven-3.5.3') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage('test stage') {
            steps{
                withMaven(maven : 'apache-maven-3.5.3') {
                    sh 'mvn test'
                }
            }
        }

        stage('install stage') {
            steps{
                withMaven(maven : 'apache-maven-3.5.3') {
                    sh 'mvn install'
                }
            }
        }

    }

}
