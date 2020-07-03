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