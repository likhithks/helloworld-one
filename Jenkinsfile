pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh "${tool name: 'sbt-1.3.4', type: 'org.jvnet.hudson.plugins.SbtPluginBuilder$SbtInstallation'}/bin/sbt compile test"
      }
    }

  }
}
