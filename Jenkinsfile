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
        sh 'pwd'
      }
    }
  }
}