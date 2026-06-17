pipeline {
    agent any

    environment {
        PATH = "/usr/local/share/dotnet/dotnet:${env.PATH}"
    }

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
    }
}