pipeline {
  agent any
  environment {
        Go111MODULE='on'
    }
  tools {
    go '1.19.3'
  }
  stages {
    stage('Tesing') {
      steps {
        git 'https://github.com/Sajjadkhan12/go-webapp-sample.git'
        sh 'go test ./...'
      }
    }

    stage('build') {
           steps {
                script{
                    image = docker.build("sajjadkhan212/go-webapp-sample")
             }
       }
     }
  }
}
