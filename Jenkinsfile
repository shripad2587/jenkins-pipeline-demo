pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Getting source code'
            }
        }

        stage('Build') {
            steps {
                sh '''
                echo "Building application..."
                sleep 10
                '''
            }
        }

        stage('Test') {
            steps {
                sh '''
                ec "Running tests..."
                sleep 10
                '''
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                echo "Deploying application..."
                sleep 10
                '''
            }
        }

    }

    post {
        success {
            echo 'Pipeline Successful'
        }

                failure {
            echo 'Pipeline Failed'

    }
}
}