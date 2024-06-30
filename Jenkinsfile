pipeline {
  agent Any
  stages {
    stage('build') {
      steps {
        sh 'npm --version'
        sh 'npm install'
        sh 'npm test'
      }
    }
  }
}