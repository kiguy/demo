pipeline {
  agent any
  stages {
    stage('Echo') {
      parallel {
        stage('Echo') {
          steps {
            sh 'echo "This is Awesome"'
          }
        }
        stage('Parallel Step') {
          steps {
            sh 'echo "Running a parallel step"'
          }
        }
      }
    }
  }
}