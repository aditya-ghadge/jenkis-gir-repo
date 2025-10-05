pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''ls -lrth
pwd
date
'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'hello linuxx'
          }
        }

        stage('testpar') {
          steps {
            echo 'echo hello word'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        sh 'df -Th'
      }
    }

  }
}