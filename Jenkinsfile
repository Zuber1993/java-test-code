pipeline {
  agent {
    docker {
      image 'nginx:latest'
      args '''-p 80:80
--name webserver'''
    }

  }
  stages {
    stage('build') {
      steps {
        sh '''
service nginx start'''
      }
    }

  }
}