pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh '''cat README.md && echo terve
 '''
          }
        }
        stage('error') {
          steps {
            sleep(unit: 'SECONDS', time: 3)
          }
        }
      }
    }
  }
}