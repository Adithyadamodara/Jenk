pipeline {
    agent any 

    stages {
        stage('Build Image') {
            steps {
                sh 'docker build -t jenkins-docker-test .'
            }
        }

        stage('Run container') {
            steps {
                sh 'docker run --rm jenkins-docker-test'
            } 
        }
    }
}
