def code
pipeline {
  agent any
  stages {
    stage('stage 1') {
      steps {
        sh 'echo "stage 1"'
        script {
           code = load 'scripts/hello.groovy'
            code.example1()
        }
      }
    }
    stage('stage 2') {
      steps {
        sh 'echo "stage 2"'
        script {
            code.example2()
        }
      }
    }
  }
}