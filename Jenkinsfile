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
        realtimeJUnit(testResults: 'target/surefire-reports/**/*.xml"')
      }
    }
  }
}