pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh "${tool name: 'sbt-0.13.17', type: 'org.jvnet.hudson.plugins.SbtPluginBuilder$SbtInstallation'}/bin/sbt compile test"
      }
    }

  }
}
