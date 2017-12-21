pipeline {
  agent any
  stages {
    stage('Sonar') {
      agent any
      steps {
        echo 'sonar is here'
      }
    }
    stage('build') {
      steps {
        echo 'message is building here'
      }
    }
    stage('Test') {
      steps {
        echo 'It is the Testing Stage'
      }
    }
  }
}