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
    stage('report') {
      steps {
        junit '\'build/reports/**/*.xml'
        realtimeJUnit(testResults: '*.xml')
      }
    }
  }
}