pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh '''pwd
ls'''
          }
        }

        stage('build') {
          steps {
            sh 'date'
          }
        }

      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test step'
          }
        }

        stage('test 1') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deloy'
      }
    }

  }
}