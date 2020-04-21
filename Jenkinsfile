pipeline {
  agent any
  triggers { cron('H/3 * * * *') }
  stages {
    stage('Build') {
      steps {
        bat 'dotnet build'
      }
    }
    stage('Deploy') {
      steps {
        bat 'dotnet run --project  ./ConsoleProject/ConsoleProject.csproj'
      }
    }
  }
}


