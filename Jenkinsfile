pipeline {
    agent any

    environment {
        JAVA_HOME = 'C:\\Program Files\\Java\\jdk-21'
        PATH = "${JAVA_HOME}\\bin;${env.PATH}"
    }

    stages {
        stage('Clone') { 
            steps {
                git url: 'https://github.com/Keerthi26099/kko.git', branch: 'main'
            }
        }

        stage('Verify Java Version') {
            steps {
                bat 'java -version'
                bat 'javac -version'
            }
        }

        stage('Build') {
            steps {
                bat 'javac H.java'
            }
        }

        stage('Run') {
            steps {
                bat 'java H'
            }
        }
    }
}
