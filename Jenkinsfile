pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Compiling'
        sh 'javac program.java'
      }
    }
    stage('Check file in directory') {
      steps {
        sh 'pwd'
        echo 'Checking file in the list'
        sh 'ls /var/lib/jenkins/workspace/Demo_master-HYLYAJ624X6E45Q6XYZ6HKHYT4F7VQU7PACKNEAMFEBEFGW3W6RQ'
      }
    }
    stage('Create .jar') {
      steps {
        echo 'Creating jar file'
        sh 'jar cvf program.jar program.class'
        echo 'Checking created file in the directory'
        sh 'ls'
      }
    }
    stage('Create manifest file') {
      steps {
        echo 'Creating manifest file'
        sh 'jar cvfe program.jar program *.class'
      }
    }
    stage('Run jar file') {
      steps {
        echo 'Running file'
        sh 'java -jar program.jar'
      }
    }
  }
}