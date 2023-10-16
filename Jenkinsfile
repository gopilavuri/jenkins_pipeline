pipeline {
  agent any
  stages {
    stage('dev') {
      parallel {
        stage('dev') {
          steps {
            echo 'development stage'
          }
        }

        stage('Test') {
          steps {
            echo 'Testing stage'
          }
        }

        stage('Plugin') {
          steps {
            echo 'Plugin stage'
          }
        }

      }
    }

    stage('QA') {
      steps {
        echo 'QA stage'
      }
    }

    stage('UAT') {
      steps {
        echo 'UAT stage'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy stage'
      }
    }

    stage('Operate') {
      steps {
        echo 'Operate'
      }
    }

  }
}