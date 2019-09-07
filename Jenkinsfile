pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          steps {
            echo 'hello pipeline'
          }
        }
        stage('stage2') {
          steps {
            build 'maven_1'
          }
        }
      }
    }
    stage('blue stage') {
      steps {
        sleep(time: 1, unit: 'SECONDS')
      }
    }
  }
}