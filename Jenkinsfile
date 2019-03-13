pipeline {
  agent any
  stages {
    stage('Check README') {
      agent any
      steps {
        fileExists 'README.md'
      }
    }
  }
}