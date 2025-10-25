pipeline {
    agent any

    stages {
        stage('Restore .Net Repository') {
            steps {
                bat 'dotnet restore'
            }
        }
        stage('Build .Net Project') {
            steps {
                bat 'dotnet build  --no-restore'
            }
        }
        stage('Unitb and Intagration Test') {
            steps {
                bat 'dotnet test --no-build --verbosity normal'
            }
        }
    }
}
