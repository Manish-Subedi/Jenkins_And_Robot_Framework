pipeline {
  agent {
    node {
      label 'windows'
    }

  }
  stages {
    stage('Build') {
      steps {
        bat 'build.bat'
      }
    }

    stage('Flash') {
      steps {
        bat 'flash.bat'
      }
    }

    stage('Initialize RobotFramework') {
      steps {
        bat 'robot --nostatusrc -v port1:$port1 -v port2:$port2 task3.robot'
      }
    }

    stage('Output') {
      steps {
        robot '.'
      }
    }

  }
}