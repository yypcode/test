pipeline {
  agent any
  stages {
    stage('update config open') {
      steps {
        sh 'ssh 172.16.1.10 sh /opt/shell/rinetd.sh open || true'
      }
    }

    stage('server start') {
      steps {
        sh 'ssh 172.16.1.10 sh /opt/shell/rinetd.sh start'
      }
    }

  }
}