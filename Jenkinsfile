pipeline {
   agent {
      docker { image 'nginx' }
   }
   stages {
      stage('Pull-image-nginx-test') { steps { sh 'docker run --rm nginx nginx -t' }}
   }
}