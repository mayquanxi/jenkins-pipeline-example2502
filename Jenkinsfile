pipeline {
   agent any
   stages {
      stage('Build') {
         steps {
            echo 'Building'
         }
      }
      stage('Checking Building') {
         steps {
            input 'Does the staging buiding look ok?'
         }
      }
      stage('Testing') {
         steps {
            echo 'Testing'
         }
      }
      stage('Deploying') {
         steps {
            echo 'Deploying'
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