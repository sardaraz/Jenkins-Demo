pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Application build stage...' 
        }
       }
        stage('Test') {
            steps {
        sh '''
          gcloud compute scp /var/lib/jenkins/workspace/Jenkins-GDC-Demo_main/README.md appserver:/var/www/html --zone=us-west4-b
        '''
      }
        }
        stage('Run') {
            steps {
                echo 'Application run stage' 
            }
        }
    }
}
