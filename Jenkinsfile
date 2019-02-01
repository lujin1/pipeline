pipeline {
  agent any
  stages {
    stage('1') {
      parallel {
        stage('1') {
          steps {
            echo '1111'
          }
        }
        stage('2') {
          steps {
            sh 'ls'
            sh 'hostname'
          }
        }
      }
    }
  }
}