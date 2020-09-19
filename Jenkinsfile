pipeline {
    agent any

    tools {
        go 'go-1.14.4'
    }

    stages {

        stage ('Install Dependencies'){
            steps {
                sh '''
                  go get github.com/instana/go-sensor
                  go get github.com/streadway/amqp
                '''
            }
        }
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