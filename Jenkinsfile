pipeline {
    agent any

    stages {
        stage('GitHub Access') {
            steps {
                script {
                    // Checkout the repository using the GitHub credentials
                    git credentialsId: 'your-credential-id', url: 'https://github.com/harshithaksherasagar/jobs21.git'
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
