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
        junit 'build/reports/**/*.xml'
        archiveArtifacts 'build/libs/**/*.jar'
      }
    }
  }
}