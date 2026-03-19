pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/christianflorea/ece-453-maven-samples', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn clean test verify'
      }
    }

  }
}