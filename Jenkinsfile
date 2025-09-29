pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed'
      }
    }

    stage('Test') {
      parallel {
        stage('Test2') {
          steps {
            echo 'Test completed'
          }
        }

        stage('Test1') {
          steps {
            echo 'Run completed'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deployment completed'
      }
    }

  }
}