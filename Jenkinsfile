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
    stage('Deploy') {
      steps {
        echo 'It is the Testing Stage'
        build 'PDNS-Stage-Deploy'
      }
    }
    stage('Test') {
      steps {
        echo 'Deploy From here'
        build 'PDNS-Regression'
      }
    }
    stage('Production') {
      steps {
        build 'PDNS-Prod'
      }
    }
  }
}