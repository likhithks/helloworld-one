pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '${tool name: \'SBT_HOME\', type: \'org.jvnet.hudson.plugins.SbtPluginBuilder$SbtInstallation\'}/usr/local/bin/sbt compile'
      }
    }

  }
}