pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Compiling Java code...'
                sh 'javac Main.java'
            }
        }
        stage('Test') {
            steps {
                echo 'Running Java program...'
                sh 'java Main'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployment step (placeholder)...'
            }
        }
    }

    post {
        always {
            echo 'This will always run after the stages.'
        }
        success {
            echo 'This will run only if the pipeline succeeds.'
        }
        failure {
            echo 'This will run only if the pipeline fails.'
        }
    }
}