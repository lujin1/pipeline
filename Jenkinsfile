pipeline {
  agent {
    kubernetes {
      label 'jenkins-node'
      containerTemplate {
        name 'jenkins-node'
        image 'gcr.io/gcp-runtimes/ubuntu_16_0_4:laster'
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
    stage('Deployment') {
      parallel {
        stage('Deployment-1') {
          steps {
            echo 'Deployment-1'
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
    stage('Map Route') {
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
    stage('Unmap Route') {
      steps {
        echo 'Unmap Route'
      }
    }
    stage('Stop Old APP') {
      steps {
        echo 'Stop Old APP'
      }
    }
    stage('Delete Old APP') {
      steps {
        echo 'Delete Old APP'
      }
    }
    stage('Smoke Test') {
      steps {
        echo 'Smoke Test'
      }
    }
    stage('1') {
      steps {
        anchore(name: 'an', bailOnPluginFail: true, engineCredentialsId: 'qweqweqwe')
      }
    }
  }
}
