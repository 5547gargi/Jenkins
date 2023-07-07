pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'This is development stage'
      }
    }

    stage('test') {
      steps {
        echo 'This is testing stage'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'This is build stage'
          }
        }

        stage('fixes') {
          steps {
            echo 'This is fix stage'
          }
        }

        stage('operate') {
          steps {
            echo 'this is operate stage'
          }
        }

        stage('prod') {
          steps {
            echo 'This is prod stage'
          }
        }

        stage('deploy') {
          steps {
            echo 'this is deploy stage'
          }
        }

      }
    }

  }
}