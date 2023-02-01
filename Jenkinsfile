pipeline {
  agent any
  stages {
    stage('hunting') {
      steps {
        sh 'echo "hello"'
        nodejs('survive_1') {
          sh 'npm install'
        }

      }
    }

    stage('build') {
      steps {
        nodejs('survive_1') {
          sh 'ng build'
        }

      }
    }

  }
}