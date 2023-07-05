pipeline {
    agent { docker { image 'node:18.16.0-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'node --version'
            }
        }
        stage('hello world') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }

    }
}