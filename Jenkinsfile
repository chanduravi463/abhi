pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'echo"this stage is build information"'
          }
        }

        stage('parallel') {
          steps {
            sh 'echo "parallel stage"'
          }
        }

      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh 'echo "this stage test information"'
          }
        }

        stage('paralell') {
          steps {
            sh 'echo "parallel stage"'
          }
        }

      }
    }

  }
}