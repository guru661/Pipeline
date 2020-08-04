pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Hello Build Completed'
          }
        }

        stage('Build1') {
          steps {
            echo 'Hello'
          }
        }

        stage('Test') {
          steps {
            echo 'Testing'
          }
        }

        stage('Verify') {
          steps {
            echo 'Verifying'
          }
        }

      }
    }

    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            echo 'Deploying to Jfrog'
          }
        }

        stage('Deploy to server') {
          steps {
            echo 'Deploying to server'
          }
        }

      }
    }

    stage('Application Restart') {
      steps {
        echo 'Restarting the appliaction'
      }
    }

  }
}
