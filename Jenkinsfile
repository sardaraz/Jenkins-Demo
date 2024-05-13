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
          gcloud compute zones list
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
