pipeline {
  agent any
  stages {
    stage('Commit Stage') {
      steps {
        echo 'Hi this is commit stage'
      }
    }

    stage('Build Stage') {
      steps {
        echo 'Hi this is build stage'
      }
    }

    stage('Test') {
      steps {
        echo 'Hi this is testing'
      }
    }

    stage('staging') {
      steps {
        echo 'Hi this is staging'
      }
    }

    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            echo 'Hi this is deploy'
          }
        }

        stage('Operate') {
          steps {
            echo 'Hi this is operate'
          }
        }

      }
    }

  }
}