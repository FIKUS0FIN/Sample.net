pipeline {
  agent {
    node {
      label 'windows'
    }

  }
  stages {
    stage('build') {
      steps {
        bat 'nuget restore'
        bat "\"${tool 'MSBuild-deff'}\""
      }
    }
  }
}
