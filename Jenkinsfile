pipeline {
    agent any
    
    stages {
        stage('Delete Existing Repository') {
            steps {
                // Delete the existing repository if it exists
                deleteDir()
            }
        }
        stage('Clone Repository') {
            steps {
                // Clone the repository
                git branch: 'main', url: 'https://github.com/sardaraz/Jenkins-Demo.git'
            }
        }
        stage('Build') {
            steps {
                // Run Python script directly without using nohup
                sh 'javac HelloWorld.java'
                sh 'java HelloWorld'
            }
        }
    }
}
