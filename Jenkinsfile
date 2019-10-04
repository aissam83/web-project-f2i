pipeline {
  agent any
  stages { 
    stage ("Init") {
    steps {
      sh '''
         mvn clean
         '''
          }
                   }
    stage ("Build") {
    steps {
    echo "Building..."
          }
                   }
    stage ("Deploy") {
    steps {
    echo "Code deployed."
          }
                   }
      }
      }
