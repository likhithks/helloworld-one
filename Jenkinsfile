pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'sh "${tool name: \'sbt\', type: \'org.jvnet.hudson.plugins.SbtPluginBuilder$SbtInstallation\'}/usr/local/bin/sbt compile"'
      }
    }

  }
}