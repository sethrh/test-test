pipeline {
  agent any
  stages {
    stage('Check README') {
      agent any
      steps {
        fileExists 'README.md'
      }
    }
    stage('Slack') {
      steps {
        slackSend(baseUrl: 'https://quantumspatial.slack.com', channel: '@seth', message: 'hi from jenkins', teamDomain: 'quantumspatial', token: 'k7oNioF06cNK6uqtFxDcIqaD')
      }
    }
  }
}