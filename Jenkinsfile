pipeline {
    agent any

    stages {
     
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
