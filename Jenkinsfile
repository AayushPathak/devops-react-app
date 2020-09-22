pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile.dev'
    }

  }
  stages {
    stage('error') {
      steps {
        sh 'docker version'
      }
    }

  }
}