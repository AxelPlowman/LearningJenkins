/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'node:18.16.0-alpine' } }
    stages {
        stage('build') {
            steps {
                
                echo 'node version: '
                version=sh 'node --version'
                echo $version
                echo 
                echo '(should be version 18.16.0)'
                if [ $version == '18.16.0' ]; then 
                    echo 'node version is the correct version!'
                else 
                    echo  'node version is not the correct version.'
                fi

            }
        }
    }
}