pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/vamsidvk09/game-of-life.git'
      }
    }
    stage('Build') {
      steps {
        sh 'mvn -B clean package'
      }
    }
  }
  environment {
    COMPELETED_MSG = 'Build done!'
  }
}