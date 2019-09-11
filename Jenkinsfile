pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'ipconfig'
      }
    }
    stage('Tests') {
      steps {
        echo 'test stage'
        bat 'ipconfig'
      }
    }
  }
}