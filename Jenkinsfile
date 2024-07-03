pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the repository
                git 'https://github.com/MELEKGEZER/webapp.git'
                
            }
        }
        stage('Build') {
            steps {
                // No build steps needed for a simple HTML page
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                // No tests for a simple HTML page
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                // Deployment steps, for example copying the file to a web server
                echo 'Deploying...'
                sh 'cp index.html /var/www/html/index.html'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished.'
        }
    }
}

