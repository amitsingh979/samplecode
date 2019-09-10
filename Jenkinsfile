pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        bat(script: 'ipconfig', returnStatus: true, returnStdout: true)
      }
    }
  }
}