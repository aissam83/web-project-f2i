pipeline {
  agent any
  stages { 
    stage ("Init") {
    steps {
    echo "Testing..."
         sh '''
         mvn clean
         mvn package
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
