pipeline {
  agent any
  stages {
    stage('Build new artifact') {
      parallel {
        stage('Build new artifact') {
          steps {
            echo 'Push to artifactory'
          }
        }
        stage('Static Code Security Analysis') {
          steps {
            echo 'bla'
          }
        }
      }
    }
    stage('Deploy to QA') {
      steps {
        echo 'Deployment to Q&A environment'
      }
    }
    stage('Deploy to Prod') {
      steps {
        echo 'Deploy to Prod env.'
      }
    }
  }
}