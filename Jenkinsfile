pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'ipconfig'
      }
    }
    stage('test') {
      steps {
        echo 'test stage'
      }
    }
    stage('Report') {
      steps {
        junit 'junit \'tests/results/*.xml\''
        junit 'target/surefire-reports/**/*.xml'
      }
    }
  }
}