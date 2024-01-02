pipeline {
  agent any
  stages {
    stage('continues build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('TEST') {
      parallel {
        stage('TEST') {
          steps {
            echo 'test step'
          }
        }

        stage('test par') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
      }
    }

  }
}