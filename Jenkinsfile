pipeline {
  agent any
  stages {
    stage('Build test image') {
      steps {
        sh 'docker build -f Dockerfile.dev . -t aayushpathak/node-test'
      }
    }

    stage('Run test') {
      steps {
        sh 'docker run --name npm_test aayushpathak/node-test npm run test -- --coverage'
      }
    }

    stage('Cleanup') {
      steps {
        sh 'docker stop npm_test && docker rm npm_test'
      }
    }

  }
}
