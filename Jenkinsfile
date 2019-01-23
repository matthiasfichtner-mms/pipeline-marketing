pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Commit new release and push to repository. Build application and push to artifactory'
      }
    }
    stage('Statische Tests') {
      parallel {
        stage('Statische Code-Analyse') {
          steps {
            echo '...'
          }
        }
        stage('Statischer Sicherheitstest') {
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
    stage('Funktionale Tests') {
      parallel {
        stage('Dynamischer Sicherheitstest') {
          steps {
            echo '_'
          }
        }
        stage('Schnittstellen-Test') {
          steps {
            echo '_'
          }
        }
        stage('Barrierefreiheits-Test') {
          steps {
            echo '_'
          }
        }
        stage('GUI-Test') {
          steps {
            echo '_'
          }
        }
      }
    }
    stage('Deploy to PERF') {
      steps {
        echo '_'
      }
    }
    stage('Nicht-funktionale Tests') {
      parallel {
        stage('Last- & Performance-Test') {
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
  }
}