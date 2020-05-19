pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/bharathyadav93/new-repo.git', branch: 'master')
      }
    }

    stage('compile') {
      steps {
        bat 'mvn clean compile'
      }
    }

    stage('build') {
      steps {
        bat 'mvn build'
      }
    }

    stage('install') {
      steps {
        bat 'mvn install'
      }
    }

  }
}