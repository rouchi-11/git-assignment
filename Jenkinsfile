pipeline {
    agent any

    tools {
        jdk 'JDK25'
    }

    stages {
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
