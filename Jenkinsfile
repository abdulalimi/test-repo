pipeline {
  agent any
  stages {
  stage('Compile-Package'){
     // Get maven home path
     def mvnHome =  tool name: 'maven-3', type: 'maven'
     sh "${mvnHome}/bin/mvn package"
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
  post {
  always {
  cleanWs()
}
}
}
