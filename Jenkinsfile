pipeline {
  agent none
  stages {
    stage('Build test image') {
      steps {
        sh 'docker build -f Dockerfile.dev -t aayushpathak/node-test'
      }
    }

    stage('Run test') {
      steps {
        sh 'docker run aayushpathak/node-test npm run test -- --coverage'
      }
    }

  }
}