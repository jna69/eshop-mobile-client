pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'dotnet build eShopOnContainers.sln'
      }
    }

    stage('Deployment') {
      steps {
        sh 'dotnet publish eShopOnContainers.sln -o var/aspnet'
      }
    }

  }
}