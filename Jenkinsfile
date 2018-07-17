pipeline {
  agent {
    node {
      label 'windows'
    }

  }
  stages {
    stage('build') {
      steps {
        bat "\"${tool 'MSBuild-deff'}\" \t:Build SampleApp.sln"
      }
    }
  }
}