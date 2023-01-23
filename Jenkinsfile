pipeline {
  agent any
  tools {
    nodejs 'node-19.4.0'
  }

  options {
    timeout(time: 2, unit: 'MINUTES')
  }

  stages {
    stage('Install dependencies') {
      steps {
        bat 'cd npm i'
      }
    }
    stage('Run tests') {
      steps {
        bat 'cd npm t'
      }
    }
  }
}
