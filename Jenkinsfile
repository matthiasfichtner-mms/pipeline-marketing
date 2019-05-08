pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Commit new release and push to repository. Build application and push to artifactory'
      }
    }
    stage('static Tests') {
      parallel {
        stage('Code Quality Test') {
          steps {
            echo '...'
          }
        }
        stage('Static Security Test') {
          steps {
            echo '...'
          }
        }
      }
    }
    stage('Deploy to STAGE') {
      steps {
        echo 'Deploy to Stage env.'
      }
    }
    stage('functional Tests') {
      parallel {
        stage('Dynamic Security Test') {
          steps {
            echo '_'
          }
        }
        stage('Usability Test') {
          steps {
            echo '_'
          }
        }
        stage('GUI Test') {
          steps {
            echo '_'
          }
        }
        stage('GUI Test on Mobile Devices') {
          steps {
            echo '-'
          }
        }
        stage('API Test') {
          steps {
            echo '-'
          }
        }
      }
    }
    stage('Deploy to PERF') {
      steps {
        echo '_'
      }
    }
    stage('non-functional Tests') {
      parallel {
        stage('Load & Performance Test') {
          steps {
            echo '_'
          }
        }
        stage('Performance Signature') {
          steps {
            echo '_'
          }
        }
      }
    }
    stage('Deploy to PROD') {
      steps {
        echo '_'
      }
    }
    stage('Intelligent Insights') {
      steps {
        echo '_'
      }
    }
  }
}