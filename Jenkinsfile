pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/AbeerSaxena/DevOps'
            }
        }
        stage('Compile and Test') {
            steps {
                sh 'mvn clean compile test'
            }
        }
        stage('Package as War') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
