pipeline {
  agent any
  environment {
        Go111MODULE='on'
    }
  
  stages {
    stage('dev') {
      steps {
        git 'https://github.com/Sajjadkhan12/go-webapp-sample.git'
        sh 'go test ./...'
      }
    }

  }
}
