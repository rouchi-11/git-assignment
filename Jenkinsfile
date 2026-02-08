pipeline {
    agent any

    tools {
        jdk 'JDK25'
    }

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                url: 'https://github.com/rouchi-11/git-assignment>.git'
            }
        }

        stage('Compile Java') {
            steps {
                bat '''
                javac src\\HelloWorld.java
                '''
            }
        }

        stage('Run Program') {
            steps {
                bat '''
                java -cp src HelloWorld
                '''
            }
        }
    }
}
