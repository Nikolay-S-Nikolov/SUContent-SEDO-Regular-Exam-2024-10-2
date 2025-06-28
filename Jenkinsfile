pipeline {
    agent any

    stages {
        stage('Checkout the project') {
            steps {
                checkout scm
            }
        } 

        stage('Build the project') {
            steps {
                bat "dotnet build"
            }
        }
        
        stage('Run tests') {
            steps {
                bat "dotnet test"
            }
        }
    }
}