pipeline {
  agent any
  stages {
    stage('Init') {
      steps {
        build job: 'first_job_TEST1'
      }
    }
    stage('Build') {
      steps {
        build job: 'P1-build-and-package'
      }
    }
    stage('Deploy') {
      steps {
        build job: 'P1-deploy-to-staging'
      }
    }
  }
}
