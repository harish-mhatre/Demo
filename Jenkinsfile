pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Compiling'
        sh 'javac program.java'
      }
    }
    stage('Compile') {
      steps {
        echo 'Show'
        sh 'pwd'
      }
    }
  }
}