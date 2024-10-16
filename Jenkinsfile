pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'pwd'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'step here'
          }
        }

        stage('test par') {
          steps {
            echo 'hi there'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
        sleep 4
      }
    }

  }
}