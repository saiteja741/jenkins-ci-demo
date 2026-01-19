pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }

    stage('Docker Build') {
      steps {
        sh 'docker build -t saiteja-jenkins-demo .'
      }
    }

    stage('Docker Images') {
      steps {
        sh 'docker images | head -5'
      }
    }
  }
}
