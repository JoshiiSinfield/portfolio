pipeline {
  agent any
  stages {
    stage('TF Plan') {
      parallel {
        stage('TF Plan') {
          steps {
            sh 'echo CDL001 TF Plan'
          }
        }
        stage('Terratest') {
          steps {
            sh 'Run some Terraform testing'
          }
        }
      }
    }
    stage('Approve') {
      steps {
        input 'Approve TF?'
      }
    }
    stage('TF Apply') {
      steps {
        sh 'echo Apply TF'
      }
    }
  }
}