pipeline {
    agent any
    triggers {
        githubPush()
    }
    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code...'
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }
        stage('Test') {
        steps {
                echo 'Running unit tests...'
            }
        }
    }
    post {
        always {
            echo 'Pipeline Project web hook1'
            
        }
    }
}
