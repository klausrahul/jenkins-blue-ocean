pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello Deploy'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Hello Test'
          }
        }

        stage('Test Parallel') {
          steps {
            echo 'Test Parallel'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Hello Deploy'
        sleep 15
      }
    }

  }
}