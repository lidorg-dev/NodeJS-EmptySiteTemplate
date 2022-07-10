pipeline {
  agent any
  stages {
    stage('checkout code') {
      parallel {
        stage('checkout code') {
          steps {
            git(url: 'git@github.com:asaf-haligua/NodeJS-EmptySiteTemplate.git', branch: 'master', credentialsId: 'github')
          }
        }

        stage('say hello to me') {
          steps {
            sh 'echo "Hello"'
          }
        }

      }
    }

    stage('Build') {
      steps {
        sh 'npm install'
      }
    }

  }
}