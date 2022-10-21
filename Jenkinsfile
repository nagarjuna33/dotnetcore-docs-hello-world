pipeline {
  agent {label 'NODEJS'}
  stages {
    stage('scm') {
    git url:  'https://github.com/GitPracticeRepo/dotnetcore-docs-hello-world.git',
      branch: 'master'
    }
  }
  stage('build') {
    steps {
    sh 'dotnet build dotnetcoresample.csproj'
    sh 'dotnet publish dotnetcoresample.csproj'
    }
  }
}
