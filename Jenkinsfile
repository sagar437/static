pipeline {
    agent any
    stages {
        stage('hello AWS') {
            steps {
                withAWS(credentials: 'aws-static', region: 'us-west-2') {
                    sh 'echo "hello KB">hello.txt'
                    s3Upload bucket: 'sagar-udacity-project-3', file: 'index.html'
                }
            }
        }
    }
}

