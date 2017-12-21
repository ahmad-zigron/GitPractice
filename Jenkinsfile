pipeline {
  agent any
  stages {
    stage('Sonar') {
      steps {
        git(url: 'git@bitbucket.org:gaditek_dpi/pdns-recursor-4.0.5.git', branch: 'refs/heads/develop')
        echo 'Here is Sonar '
      }
    }
  }
}