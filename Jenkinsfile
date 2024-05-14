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
          gcloud compute copy-files /var/lib/jenkins/workspace/Jenkins-GDC-Demo_main/README.md appserver: /var/www/html --zone=us-west4-b
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
