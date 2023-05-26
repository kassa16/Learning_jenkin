pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/kassa16/Learning_jenkin', branch: 'main')
      }
    }

    stage('Log') {
      parallel {
        stage('Log') {
          steps {
            sh 'ls -al'
          }
        }

        stage('parallel') {
          steps {
            sh 'echo "This is a test to show that I can run two or more steps in parallel." "'
          }
        }

      }
    }

  }
}