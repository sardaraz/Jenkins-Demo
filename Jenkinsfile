pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'mvn -B -DskipTests clean package' 
            }
            steps {
                bat 'javac HelloWorld.java'
            }
        }
        stage('Run') {
            steps {
                bat 'java HelloWorld'
            }
        }
    }
}
