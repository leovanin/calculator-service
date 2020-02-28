pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean package'
      }
    }

    stage('Test') {
      steps {
        sh 'mvn clean test'
      }
    }

    stage('Deploy') {
      steps {
        sh 'mvn clean deploy'
      }
    }

  }
  environment {
    localhost = 'localhost'
  }
}