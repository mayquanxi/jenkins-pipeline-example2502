pipeline {
   agent any
   stages {
   	  stage('Print date to file in') {
         steps {
         	timeout(time: 1, unit: 'MINUTES') {
         		retry(5) {
         			bash 'date >> new_file2'
         		}
         	}
         }
   	  }
   }
}