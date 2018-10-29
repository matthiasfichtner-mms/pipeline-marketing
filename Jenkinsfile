pipeline {
  agent any
  stages {
    stage('Build new artifact') {
      steps {
        echo 'Commit new release and push to repository. Build application and push to artifactory'
      }
    }
    stage('Code Quality Test') {
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
    stage('Deploy to Stage') {
      steps {
        echo 'Deploy to Stage env.'
      }
    }
    stage('Dynamic Security Test') {
      parallel {
        stage('Dynamic Security Test') {
          steps {
            echo '_'
          }
        }
        stage('API Test') {
          steps {
            echo '_'
          }
        }
        stage('API Simulation') {
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
      }
    }
    stage('Deploy to Perform') {
      steps {
        echo '_'
      }
    }
    stage('Load & Performance Test') {
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
    stage('Deploy to Prod') {
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