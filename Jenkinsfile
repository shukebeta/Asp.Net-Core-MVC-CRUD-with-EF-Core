pipeline {
  agent any
  triggers { pollSCM('H/5 * * * *') }
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


