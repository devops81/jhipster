pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo Build'
      }
    }

    stage('Backend') {
      parallel {
        stage('Backend') {
          steps {
            sh 'echo Backend'
          }
        }

        stage('Performance') {
          steps {
            sh 'echo Performance'
          }
        }

      }
    }

    stage('Frontend') {
      steps {
        sh 'echo Frontend'
      }
    }

    stage('Static Analysis') {
      steps {
        sh 'echo Static analysis'
      }
    }

    stage('Deploy') {
      steps {
        sh 'echo Deploy'
      }
    }

  }
}