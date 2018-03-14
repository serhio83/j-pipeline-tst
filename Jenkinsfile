pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            sh 'pwd'
          }
        }
        stage('parallel stage1') {
          steps {
            echo 'It works in parallel'
          }
        }
      }
    }
    stage('stage 2') {
      steps {
        sh 'ls -la'
      }
    }
  }
}