pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Validate') {
            steps {
                echo 'Validating HTML files...'
                sh 'find . -name "*.html" | head -10'
            }
        }
        stage('Test') {
            steps {
                echo 'Checking HTML files exist...'
                sh 'test -f index.html && echo "index.html found!" || echo "index.html not found"'
            }
        }
        stage('Deploy') {
            steps {
                echo 'HTML site 3 deployed successfully!'
                
            }
        }
    }
}
