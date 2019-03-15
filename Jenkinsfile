pipeline {
  agent any
  stages {
    stage('Check README') {
      agent any
      steps {
        fileExists 'README.md'
      }
    }
    stage('Unittest') {
      steps {
        sh 'tox'
      }
    }
  }
}