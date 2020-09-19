pipeline {
    agent any

    tools {
        go 'go-1.14.4'
    }

    stages {
        stage('Compile Code') {
            steps {
                sh '''
                    cd src
                    go build
                '''
            }

        }

    }

}