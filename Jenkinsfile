
pipeline {
    agent { docker { image 'golang:1.17.5-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'curl -fsSL https://get.docker.com -o get-docker.sh'
                sh 'go build main.go'
                sh 'go run main'
            }
        }
        stage('test') {
            steps {
                sh 'go test'
            }
        }
    }
}

