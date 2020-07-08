pipeline {
  agent any

  tools {
    go 'go-1.14'
  }

  stages {

    stage('Install Dependencies') {
      steps {
        sh '''
          go get github.com/instana/go-sensor
          go get github.com/streadway/amqp
          
          
        '''
      }
    }

    stage('Lint Code') {
      steps {
        sh '''
          go get -u golang.org/x/lint/golint
          ~/go/bin/golint src/main.go
        '''
      }
    }

    stage('Compile COde') {
      steps {
        sh '''
          cd src
          go build
        '''
      }
    }

  }

}