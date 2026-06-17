pipeline {
    agent any

    stages {
        stage("Restore Packages"){
            steps {
                sh 'dotnet restore'
            }
        }
        stage("Build Project"){
            steps {
                sh 'dotnet build'
            }
        }
        stage("Run Tests"){
            steps {
                sh 'dotnet test'
            }
        }
        stage("Run Tests"){
            steps {
                sh 'dotnet test'
            }
        }
    }
}