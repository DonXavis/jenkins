pipeline {
  agent any
  stages {
    stage('paso 1') {
      steps {
        script {
          sh "echo 'hola mundo'"
        }

        echo 'Hola mundo'
      }
    }

  }
  environment {
    cloudbees = 'variable'
  }
  post {
    always {
      deleteDir()
      sh 'echo \'fase always\''
    }

    success {
      sh 'echo \'fase success\''
    }

    failure {
      sh 'echo \'fase failure\''
    }

  }
}