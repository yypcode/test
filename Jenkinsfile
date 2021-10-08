pipeline {
  agent {
    docker {
      image 'docker pull nginx:stable'
    }

  }
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh 'echo "yyping"'
            sh 'echo "yyping234"'
          }
        }

        stage('test2') {
          steps {
            sleep 30
          }
        }

      }
    }

    stage('build') {
      steps {
        sh 'echo "999999"'
      }
    }

  }
}