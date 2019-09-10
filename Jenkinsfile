pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat(script: 'get Ipconfig', encoding: 'Ipconfig', returnStatus: true, returnStdout: true)
      }
    }
  }
}