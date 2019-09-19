pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello from Core / Jenkins!'
      }
    }
    stage('Testing') {
      steps {
        sh 'sleep 5'
        sh 'echo Tests completed!'
      }
    }
    stage('Publish Event') {
      steps {
        script {
          publishEvent simpleEvent('testingCompleted')
        }

      }
    }
  }
}