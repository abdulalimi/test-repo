pipeline {
  agent any
  environment {
BUILD_SCRIPTS_GIT="http://10.100.100.10:7990/scm/~myname/mypipeline.git"
BUILD_SCRIPTS='mypipeline'
BUILD_HOME='/var/lib/jenkins/workspace'

}
  stages {
  stage('Build'){
    steps {
     sh "/Users/alimia/apache-maven-3.5.4/bin/mvn"
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
  post {
  always {
  cleanWs()
}
}
}
