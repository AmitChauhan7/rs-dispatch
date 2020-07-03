pipeline {
  agent any

  tools {
    go 'go-1.14'
  }

  stages {

    stage('Compile COde') {
      steps {
        sh '''
          cd src
          go compile
        '''
      }
    }

  }

}