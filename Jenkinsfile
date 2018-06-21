pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo Build'
      }
    }
    stage('Backend') {
      parallel {
        stage('Unit Test') {
          steps {
            sh 'echo Unit'
          }
        }
        stage('Performance') {
          steps {
            sh 'echo Performance'
          }
        }
      }
    }
    stage('Static Analysis') {
      steps {
        sh 'echo Static analysis'
      }
    }
    stage('Deployment') {
      steps {
        sh 'echo Deployment'
      }
    }
  }
}