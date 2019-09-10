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
        bat(script: 'cp -r app/build/test-results $WORKSPACE/test-results', returnStatus: true, returnStdout: true)
        junit '**/test-results/**/*.xml'
      }
    }
  }
}