pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
date'''
        sh '''pwd 
date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'testing'
          }
        }

        stage('test1') {
          steps {
            echo 'parallel testing'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploying'
      }
    }

  }
}