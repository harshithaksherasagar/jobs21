pipeline {
    agent any

    stages {
        stage('GitHub Access') {
            steps {
                script {
                    // Checkout the repository using the GitHub credentials
                    git credentialsId: '2a21f3f4-24c4-4f05-8dfa-e81d25dc9798', url: 'https://github.com/harshithaksherasagar/jobs21.git'
                }
            }
        }
        stage('Java Program Execution') {
            steps {
                script {
                    // Compile and run the Java program
                    sh 'javac HelloWorld.java'
                    sh 'java HelloWorld'
                }
            }
        }
        stage('Python Program Execution') {
            steps {
                script {
                    // Run the Python program
                    sh 'python hello.py'
                }
            }
        }
    }
}
