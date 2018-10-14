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
  }
  environment {
    COMPELETED_MSG = 'Build done!'
  }
}