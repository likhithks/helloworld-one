pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''${tool name: \'sbt\', type: \'org.jvnet.hudson.plugins.SbtPluginBuilder$SbtInstallation\'}/bin/sbt clean
${tool name: \'sbt\', type: \'org.jvnet.hudson.plugins.SbtPluginBuilder$SbtInstallation\'}/bin/sbt compile
${tool name: \'sbt\', type: \'org.jvnet.hudson.plugins.SbtPluginBuilder$SbtInstallation\'}/bin/sbt package'''
      }
    }

    stage('post_build') {
      steps {
        sh 'scp /var/jenkins_home/workspace/sbt_helloWorld_demo/target/scala-2.12/hello_2.12-0.1.0-SNAPSHOT.jar shenoyl@g4t7470.houston.hpecorp.net:/HDFS_ROOT/EA/supplychain/oozie/apiconnectivity'
      }
    }

  }
}