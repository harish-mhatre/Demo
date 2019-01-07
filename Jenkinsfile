pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Compiling'
        sh 'javac program.java'
      }
    }
    
    stage('Display') {
      steps {
      echo 'Show'
      sh 'java program';
    }
    }
   }
}
