pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Allication build stage...' 
        }
       }
        stage('Test') {
            steps {
        sh '''
          gcloud version
        '''
      }
        }
        stage('Run') {
            steps {
                echo 'Allication run stage' 
            }
        }
    }
}
