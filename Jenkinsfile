/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'node:18.16.0-alpine' } }
    stages {
        stage('build') {
            steps {
                
                echo 'node version: '
                sh 'node --version'
                echo 
                echo '(should be version 18.16.0)'
            }
        }
    }
}