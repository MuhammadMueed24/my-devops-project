pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/MuhammadMueed24/my-devops-project.git'
            }
        }
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t myapp:latest .'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Running tests... (placeholder)"'
            }
        }
        stage('Deploy Container') {
            steps {
                sh '''
                  docker stop myapp || true
                  docker rm myapp || true
                  docker run -d -p 5000:5000 --name myapp myapp:latest
                '''
            }
        }
    }
}
