pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'export name=likhith'
      }
    }

    stage('read_var') {
      steps {
        sh 'echo $name'
      }
    }

  }
}