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
      steps {
        sh 'hostname -a'
      }
    }
  }
}