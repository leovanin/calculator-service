pipeline {
  agent none
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean test'
      }
    }

  }
  environment {
    localhost = 'localhost'
  }
}