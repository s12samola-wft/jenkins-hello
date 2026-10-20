pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the app...'
                sh 'ls -la'
                sh 'mkdir -p build && echo "app v1" > build/app.txt'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing the app...'
                sh 'grep "app v1" build/app.txt'
            }
        }
    }
}
