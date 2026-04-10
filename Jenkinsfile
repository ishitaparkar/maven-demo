pipeline {
    agent any
    tools {
        maven 'Maven'
    }
    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/ishitaparkar/maven-demo.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean compile'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}