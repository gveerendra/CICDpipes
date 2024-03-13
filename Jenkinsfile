pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'dev1'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test1'
          }
        }

        stage('prod') {
          steps {
            echo 'prod1'
          }
        }

        stage('dep') {
          steps {
            echo 'dep'
          }
        }

      }
    }

  }
}