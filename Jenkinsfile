pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // TODO: Build step
                sh './gradlew assemble'
            }
        }
        stage('Test') {
            steps {
                // TODO: Test step
                sh './gradlew test'
            }
        }
    }
    post {
        success {
            echo 'Build and tests were successful!'
        }
        failure {
            echo 'Build or tests failed. Please investigate.'
        }
    }
}
