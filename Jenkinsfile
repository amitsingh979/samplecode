pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'ipconfig'
      }
    }
    stage('Test') {
      environment {
        CI = 'true'
      }
      steps {
        sh './Test-1.bat'
      }
    }
    stage('Report') {
      steps {
        junit '**/build/test-reports/*.xml'
      }
    }
  }
}