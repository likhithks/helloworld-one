pipeline {
  agent any
  stages {
    stage('Initial_build') {
      steps {
        sh '"${tool name: \'sbt\', type: \'org.jvnet.hudson.plugins.SbtPluginBuilder$SbtInstallation\'}/bin/sbt clean"'
      }
    }

  }
}