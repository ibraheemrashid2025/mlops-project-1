pipeline {
    agent any
    stages {
        stage('Build') {
            steps { sh 'docker build -t app .' } // Docker image banaye ga
        }
        stage('Test') {
            steps { sh 'docker images' } // Images ki list check kare ga
        }
        stage('Deploy') {
            steps { sh 'docker run -d -p 80:80 app' } // Container on kare ga
        }
    }
}
