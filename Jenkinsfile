pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'hello world ..!'
          }
        }

        stage('Test') {
          steps {
            echo 'Testing the application'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying the APP'
      }
    }

  }
}