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
        sh 'ls /var/lib/jenkins/workspace/Demo_master-HYLYAJ624X6E45Q6XYZ6HKHYT4F7VQU7PACKNEAMFEBEFGW3W6RQ'
      }
    }
    stage('Create .jar') {
      steps {
        sh 'jar cvmf program.jar manifest.mf  program.class'
        sh 'ls'
      }
    }
    stage('Run jar file') {
      steps {
        sh 'java -jar program.jar'
      }
    }
  }
}