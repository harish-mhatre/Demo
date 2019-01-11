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
        sh 'jar cvf program.jar program.class'
        sh 'ls'
      }
    }
    stage('Create manifest file') {
      steps {
        sh 'jar cvfe program.jar program *.class'
        sh 'java -jar program.jar'
      }
    }
  }
}