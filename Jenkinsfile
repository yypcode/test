pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sh '''echo $abc
echo $ab
echo $dd'''
      }
    }

  }
  environment {
    abc = '123'
    ab = '12'
    dd = 'a'
  }
}