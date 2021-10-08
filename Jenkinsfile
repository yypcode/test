pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('git') {
      steps {
        git 'https://github.com/yyp2021/test.git'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            sleep 300
          }
        }

        stage('test2') {
          steps {
            sh '''echo $abc
echo $ab'''
          }
        }

      }
    }

  }
  environment {
    abc = '123'
    ab = '321'
  }
}