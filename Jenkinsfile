pipeline {
  agent any
  stages {
    stage('Echo') {
      parallel {
        stage('Echo') {
          steps {
            sh 'ONE="This is Awesome"'
          }
        }
        stage('Parallel Step') {
          steps {
            sh 'TWO="Parallel Step"'
          }
        }
      }
    }
    stage('') {
      steps {
        sh 'echo "One is: ${ONE} and two is: ${TWO}"'
      }
    }
  }
}