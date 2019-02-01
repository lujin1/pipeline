pipeline {
    agent {
    label "jenkins-maven"
  }
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
    stage('11') {
      parallel {
        stage('11') {
          steps {
            sh 'hostname -a'
          }
        }
        stage('22') {
          steps {
            echo '222'
          }
        }
      }
    }
  }
}
