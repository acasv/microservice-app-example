pipeline {
  agent any
  stages {
    stage('Microservices Build') {
      steps {
        echo 'Api Build Succesfully'
      }
    }

    stage('Auth-Api Test') {
      parallel {
        stage('Auth-Api Test') {
          steps {
            echo 'Test Completed'
          }
        }

        stage('Users-Api Test') {
          steps {
            echo 'Test Completed'
          }
        }

        stage('Todos-Api Test') {
          steps {
            echo 'Test Completed'
          }
        }

        stage('Log-message Test') {
          steps {
            echo 'Test Completed'
          }
        }

      }
    }

    stage('Artifact Construction') {
      steps {
        echo 'Artifact Constructed'
      }
    }

  }
}