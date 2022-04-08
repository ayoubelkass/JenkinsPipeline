pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Building the APP'
          }
        }

        stage('Test') {
          steps {
            echo 'Testing the application'
            echo "Get the Path ${ChromeDriverPath}"
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
  environment {
    ChromeDriverPath = 'Documents'
  }
}