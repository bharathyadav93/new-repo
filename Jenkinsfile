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

  }
}