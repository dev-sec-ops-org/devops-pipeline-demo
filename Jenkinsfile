pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        script {
          echo 'Building Images ...'
          def buildArgs = """-f src/Dockerfile \
          ."""
          docker.build("devop-pipeline:v1.0.1", buildArgs)
        }
      }
    }
    stage('Test') {
      steps {
        echo 'Testing...'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying...'
      }
    }
  }
}
