pipeline {
  agent any
  stages {
    stage('Sonar') {
      agent any
      steps {
        git(url: 'git@bitbucket.org:gaditek_dpi/pdns-recursor-4.0.5.git', branch: 'refs/heads/develop')
        echo 'Here is Sonar '
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