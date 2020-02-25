pipeline {
   agent any
   stages {
      stage('No-op') {
         steps {
            sh 'ls -be'
         }
      }
   }
   post {
      always {
         echo 'One way or another, I have finished'
         deleteDir() /* clean up our workspace */
      }
      success {
         echo 'I am Unstable :/'
      }
      failure {
         echo 'I failed :('
      }
      changed {
         echo 'Things were different before...'
      }
   }
}