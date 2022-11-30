pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        echo 'Building Images ...'
        script {
          def buildArgs = """-f Dockerfile ."""
          docker.build("devop-pipeline:v1.0.0.2", buildArgs)
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
