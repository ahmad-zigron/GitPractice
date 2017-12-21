pipeline {
  agent any
  stages {
    stage('Sonar') {
      agent any
      steps {
        echo 'sonar is here'
        build 'PDNS-Sonar'
      }
    }
    stage('build') {
      steps {
        echo 'message is building here'
        build 'PDNS-Build'
      }
    }
    stage('Test') {
      steps {
        echo 'It is the Testing Stage'
        build 'PDNS-Stage-Deploy'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy From here'
      }
    }
  }
}