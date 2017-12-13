pipeline {
  agent any
  stages {
    stage('stage 1') {
      steps {
        echo 'On stage 1'
      }
    }
    stage('stage 2') {
      steps {
        parallel(
          "stage 2": {
            echo 'on stage 2'
            
          },
          "": {
            bat 'javac SampleJavaProject.java SampleJavaProject'
            
          }
        )
      }
    }
  }
}