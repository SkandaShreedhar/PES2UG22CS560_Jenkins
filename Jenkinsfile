pipeline {
    agent any  // Runs on any available agent

    stages {
        stage('Build') {
            steps {
                script {
                    // sh 'g++ -o hello_exec main/hello.cpp' // Compiles the C++ file
                }
            }
        }

        stage('Test') {
            // steps {
                // script {
                    sh './hello_exec'  // Runs the compiled executable
                }
            }
        }

        // stage('Deploy') {
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
