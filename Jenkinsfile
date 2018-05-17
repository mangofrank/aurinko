pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh '''cat README.md
&& echo '''
          }
        }
        stage('') {
          steps {
            sleep(unit: 'SECONDS', time: 3)
          }
        }
      }
    }
    stage('') {
      steps {
        mail(subject: 'terve', body: 'Moikka, Mitäs kuuluu? T kurssikaveri', from: 'jarmo.kalsi@gmail.com', to: 'ville.hedstrom@gmail.com')
      }
    }
  }
}