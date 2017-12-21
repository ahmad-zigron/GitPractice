pipeline {
  agent any
  stages {
    stage('Sonar') {
      agent any
      steps {
        echo 'sonar is here'
        node {
          checkout scm
        sh './script.sh'
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
