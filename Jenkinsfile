pipeline {
  agent any
  stages {
    stage('git scm update') {
      steps {
        git url: 'https://github.com/IaC-Sources/echo-ip.git', branch: 'main'
      }
    }   
    stage('docker build and push') {
      steps {
        script {
          sh 'echo build'
        }
      }
    }
    stage('deploy kubernetes') {
      steps {
        sh '''
          echo 'deploy'
        '''
      }
    }
  }
}
