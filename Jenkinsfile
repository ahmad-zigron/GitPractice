pipeline {
  agent any
  stages {
    stage('Sonar') {
      node {
        checkout scm
      agent any
      steps {
        echo 'sonar is here'
       }
      }
    }
    stage('build') {
      steps {
        echo 'message is building here'
      }
    }
    stage('Deploy') {
      steps {
        echo 'It is the Deploy Stage'
      }
    }
    stage('Test') {
      steps {
        echo 'Test goes here'
      }
    }
    stage('Production') {
      steps {
        echo 'Production goes here'
      }
    }
  }
}
