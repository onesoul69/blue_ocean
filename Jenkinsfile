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
            echo '*Testing*'
          }
        }

        stage('Parallel') {
          steps {
            echo '*Running Environment*'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo '*Building Environment*'
      }
    }

    stage('Final') {
      steps {
        echo '*Clean-Up*'
      }
    }

  }
}