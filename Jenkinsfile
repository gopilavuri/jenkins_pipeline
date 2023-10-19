pipeline {
  agent any
  stages {
    stage('git checkout') {
      steps {
        echo 'development stage'
        git(url: 'https://github.com/gopilavuri/SimpleWebApp.git', branch: 'master')
      }
    }

    stage('sonarqube') {
      steps {
        echo 'QA stage'
      }
    }

    stage('Build') {
      steps {
        echo 'UAT stage'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy stage'
      }
    }

    stage('slack') {
      steps {
        slackSend()
      }
    }

  }
}