pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile.dev'
    }

  }
  stages {
    stage('') {
      steps {
        sh 'docker build -f Dockerfile.dev .'
      }
    }

  }
}