pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Build step'
        bat 'echo "%date%"'
      }
    }

    stage('Deploy Stage') {
      parallel {
        stage('Deploy Stage') {
          steps {
            echo 'Deploy Stage'
          }
        }

        stage('Deploy Parallel') {
          steps {
            echo 'Deploy Parallel'
          }
        }

      }
    }

    stage('Deploy Prod') {
      steps {
        echo 'Deploy Prod'
      }
    }

    stage('') {
      steps {
        input(message: 'Shall we continue', ok: 'Yes we should')
      }
    }

  }
}