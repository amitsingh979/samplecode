pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'ipconfig'
      }
    }
    stage('Tests') {
      parallel {
        stage('Tests') {
          steps {
            echo 'test stage'
            bat 'ipconfig'
          }
        }
        stage('Test 2') {
          steps {
            echo 'Test 2'
          }
        }
        stage('Test 3') {
          steps {
            echo 'Test 3'
          }
        }
        stage('Test 4') {
          steps {
            echo 'Test 3'
          }
        }
      }
    }
  }
}