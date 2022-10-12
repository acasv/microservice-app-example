pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Auth build') {
          steps {
            echo 'auth built'
          }
        }

        stage('Users build') {
          steps {
            echo 'Users Built'
          }
        }

        stage('Todos build') {
          steps {
            echo 'Todos built'
          }
        }

        stage('Log build') {
          steps {
            echo 'Log built'
          }
        }

        stage('Front build') {
          steps {
            echo 'Front built'
          }
        }

      }
    }

    stage('Testing') {
      parallel {
        stage('Auth Test') {
          steps {
            echo 'auth completed'
          }
        }

        stage('Users Test') {
          steps {
            echo 'Users completed'
          }
        }

        stage('Todos Test') {
          steps {
            echo 'Todos completed'
          }
        }

        stage('Log Test') {
          steps {
            echo 'Log completed'
          }
        }

        stage('Front Test') {
          steps {
            echo 'Front completed'
          }
        }

      }
    }

    stage('Artifact Construction') {
      steps {
        echo 'Artifact Created'
      }
    }

  }
}