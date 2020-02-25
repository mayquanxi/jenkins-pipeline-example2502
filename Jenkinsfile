pipeline {
   agent {
      label '!windows'
   }
   environment {
      DISABLE_AUTH = 'true'
      DB_ENGINE = 'sqlite'
   }
   stages {
      stage('Build') {
         steps {
            echo "Database engine is ${DB_ENGINE}"
            echo "Disable auth is ${DISABLE_AUTH}"
            sh 'printenv'
         }
      }
   }
}