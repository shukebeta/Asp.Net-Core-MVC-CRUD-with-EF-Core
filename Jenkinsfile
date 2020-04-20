pipeline {
  agent any
  environment {
    dotnet = "C:\\Program Files\\dotnet\\dotnet.exe"
    sh = "C:\\Program Files\\Git\\bin\\sh.exe"
    nohup = "C:\\Program Files\\Git\\usr\\bin\\nohup.exe"
    PATH = "C:\\Program Files\\Git\\usr\\bin;C:\\Program Files\\Git\\bin;${env.PATH}"
  }
  stages {
    stage('build') {
      steps {
        sh 'dotnet build'
      }
    }
  }
}


