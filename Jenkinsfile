pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'hello'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            sh 'python --version'
          }
        }

        stage('test') {
          steps {
            echo 'test'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'deploy'
      }
    }

  }
}