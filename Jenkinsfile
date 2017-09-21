pipeline {
  agent any
  stages {
    stage('Inicializar') {
      steps {
        echo 'Hello World'
      }
    }
    stage('Data') {
      steps {
        parallel(
          "Data": {
            sh 'date --rfc-2822'
            
          },
          "Sleep": {
            sleep 6
            
          }
        )
      }
    }
    stage('Finalizar') {
      steps {
        echo 'Terminamos'
      }
    }
  }
}