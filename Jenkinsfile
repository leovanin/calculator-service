pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean package'
      }
    }

    stage('Run') {
      steps {
        sh 'mvn spring-boot:run'
        sh 'mvn spring-boot:stop'
      }
    }

  }
  environment {
    localhost = 'localhost'
  }
}