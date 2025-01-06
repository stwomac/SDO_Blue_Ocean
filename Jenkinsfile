pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo '"testing"'
          }
        }

        stage('parallel') {
          steps {
            echo 'parallel running'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo 'building'
      }
    }

    stage('clean up') {
      steps {
        echo 'clean environment'
      }
    }

  }
}