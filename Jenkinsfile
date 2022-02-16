
Jenkinsfile (Declarative Pipeline)

pipeline {
    agent { docker { image 'golang:1.17.5-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'go build main.go'
                sh 'go run main'
            }
        }
        stage('build') {
            steps {
                sh 'go build main.go'
                sh 'go run main'
            }
        }
    }
}

