pipeline {
    agent any

    tools {
        maven 'Maven 3.8.6' // or whatever Maven version is installed on your Jenkins
        jdk 'JDK 1.8'       // or your preferred JDK version
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build & Test') {
            steps {
                sh 'mvn clean test'
            }
        }
    }

    post {
        always {
            junit 'target/surefire-reports/*.xml'
        }
    }
}