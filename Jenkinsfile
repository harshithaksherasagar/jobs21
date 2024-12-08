pipeline {
    agent any

    stages {
        // Stage 1: GitHub access (checkout the repository)
        stage('GitHub Access') {
            steps {
                script {
                    // Checkout the repository (you'll add your GitHub URL here)
                    git 'https://github.com/yourusername/your-repository.git' 
                    // Alternatively, if Jenkins has SCM configuration:
                    // checkout scm 
                }
            }
        }

        // Stage 2: Java program execution
        stage('Java Program Execution') {
            steps {
                script {
                    // Compile and run the Java program
                    sh 'javac HelloWorld.java'
                    sh 'java HelloWorld'
                }
            }
        }

        // Stage 3: Python program execution
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
