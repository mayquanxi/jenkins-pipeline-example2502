pipeline {
   agent {
      docker { image 'nginx:alpine' }
   }
   stages {
      stage('Pull-image-nginx-test') { steps { sh 'nginx -t' }}
   }
}