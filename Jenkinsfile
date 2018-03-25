pipeline {
  agent none
  stages {
    stage('STARTUP') {
      parallel {
        stage('STARTUP') {
          steps {
            sh 'echo "hello"'
          }
        }
        stage('DEPLOY') {
          steps {
            bat(script: 'dir', encoding: 'echo "toto"', returnStatus: true, returnStdout: true)
          }
        }
      }
    }
    stage('test') {
      steps {
        sleep 11
      }
    }
  }
}