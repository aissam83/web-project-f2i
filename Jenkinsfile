pipeline {
  agent any
  stages { 
    stage ("Init") {
    steps {
    echo "Testing."
          }
                   }
    stage ("Build") {
    steps {
    echo "Building..."
      bat 'mvn clean package'
          }
      post {
        success {
          echo 'Now Archiving...'
          archiveArtifacts artifacts: '**/target/*.war'
                }
          }
                   }
    stage ("Deploy") {
    steps {
      sleep 60
      build job: 'deploy'
    echo "Code deployed."
          }
                   }
      }
      }
