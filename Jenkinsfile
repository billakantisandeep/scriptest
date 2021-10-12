pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo \'Sandeep hello world\''
      }
    }

    stage('build2') {
      parallel {
        stage('build2') {
          steps {
            sh 'echo \'Another step\''
          }
        }

        stage('test') {
          steps {
            sh 'echo \'Test cases\''
          }
        }

      }
    }

  }
}