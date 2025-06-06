pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git url: 'https://github.com/Keerthi26099/kko.git'
            }
        }

        stage('Build') {
            steps {
                bat '''
                    cd src
                    javac K.java
                '''
            }
        }

        stage('Run') {
            steps {
                bat '''
                    cd src
                    java K
                '''
            }
        }
    }
}
