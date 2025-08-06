
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                bat 'dotnet build'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'dotnet test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                bat 'dotnet publish -c Release'
            }
        }
    }
}
