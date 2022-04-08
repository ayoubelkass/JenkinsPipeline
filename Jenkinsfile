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
        input(message: 'would you like to continue ? ', id: 'ok')
        echo 'Deploying the APP'
      }
    }

  }
  environment {
    ChromeDriverPath = 'Documents'
  }
}