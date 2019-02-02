pipeline {
  agent {
    kubernetes {
      label 'jenkins-node'
      containerTemplate {
        name 'jenkins-node'
        image 'wpacr.azurecr.io/jenkins-alpinenode:v3'
        ttyEnabled true
      }

    }

  }
  stages {
    stage('Check APPs') {
      steps {
        echo '1111'
      }
    }
    stage('Deployment-1') {
      parallel {
        stage('Deployment-1') {
          steps {
            sh 'hostname -a'
          }
        }
        stage('Deployment-2') {
          steps {
            echo 'Deployment-2'
          }
        }
        stage('Deployment-3') {
          steps {
            echo 'Deployment-3'
          }
        }
        stage('Deployment-n') {
          steps {
            echo 'Deployment-n'
          }
        }
      }
    }
    stage('Check Deploy') {
      steps {
        echo '1'
      }
    }
    stage('Rollback') {
      steps {
        echo 'Rollback'
      }
    }
    stage('Map Route-1') {
      parallel {
        stage('Map Route1') {
          steps {
            echo '22'
          }
        }
        stage('Map Route-2') {
          steps {
            echo 'Map Route-2'
          }
        }
        stage('Map Route-3') {
          steps {
            echo 'Map Route-3'
          }
        }
      }
    }
  }
}