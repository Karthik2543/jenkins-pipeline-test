pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/<your-username>/jenkins-pipeline-test.git'
            }
        }
        stage('Build') {
            steps {
                echo "Simulating build..."
                sh 'chmod +x app/hello.sh'
                sh './app/hello.sh'
            }
        }
        stage('Test') {
            steps {
                echo "Running simple test..."
                sh 'echo "Tests passed successfully!"'
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying to staging..."
            }
        }
    }
}
