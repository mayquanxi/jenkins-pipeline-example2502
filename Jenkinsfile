pipeline {
   agent any
   stages {
   	  stage('Print date to file in') {
         steps {
         	timeout(time: 1, unit: 'MINUTES') {
         		retry(5) {
         			sh 'date >> /tmp/new_file2'
         		}
         	}
         }
   	  }
   }
}