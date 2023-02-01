pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
date
'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'teststep'
          }
        }

        stage('testpar') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
        sleep 10
      }
    }

  }
}