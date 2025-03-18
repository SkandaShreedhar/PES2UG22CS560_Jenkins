pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o hello_exec main/hello.cpp'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './hello_exec'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment step (Placeholder, as this is a basic pipeline)'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed!'
        }
    }
}
