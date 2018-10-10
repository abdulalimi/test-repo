pipeline {
  agent any
  stages {
    stage('Stage 1') {
      steps {
        sh 'echo SCM Checkout'
      }
    }
    stage('Build') {
      steps {
        sh 'echo Build'
      }
    }
    stage('Fetch from S3') {
      steps {
        sh 'echo Fetch from S3'
      }
    }
    stage('Spin up tidal') {
      steps {
        sh 'echo Spin up tidal instance'
      }
    }
    stage('execute code') {
      steps {
        sh 'echo Execute code'
      }
    }
  }
}
