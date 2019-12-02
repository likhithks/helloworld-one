pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''export name=likhith
echo $name "shenoy"'''
      }
    }

    stage('read_var') {
      steps {
        sh 'echo $name "shenoy"'
      }
    }

  }
}