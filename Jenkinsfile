
/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'node:18.16.0-alpine' } }
    stages {
        stage('build') {
            steps {
                script {
                    echo 'node version:'
                    def version = sh(script: 'node --version', returnStdout: true).trim()
                    echo version
                    echo
                    echo '(should be version 18.16.0)'
                    if (version == 'v18.16.0') {
                        echo 'node version is the correct version!'
                    } else {
                        echo 'node version is not the correct version.'
                    }
                }
            }
        }
    }
}