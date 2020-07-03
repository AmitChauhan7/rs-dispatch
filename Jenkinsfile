pipeline {
  agent any

  tools {
    golang 'go-1.14.4'
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