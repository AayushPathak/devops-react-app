pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile.dev'
    }

  }
  stages {
    stage('test') {
      steps {
        sh 'node --version'
      }
    }

  }
}