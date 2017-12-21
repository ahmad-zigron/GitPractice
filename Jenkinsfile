pipeline {
  agent any
  stages {
    stage('Sonar') {
      agent any
      steps {
        echo 'sonar is here'
      }
    }
    stage('pdns-build') {
      steps {
        sh './puredns_stag_build.sh'
        build 'PDNS-Stage-Deploy'
      }
    }
  }
}