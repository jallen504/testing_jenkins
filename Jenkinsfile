pipeline {
  agent any
  
  
  stages {
    stage('Setup') {
      steps {
        sh 'pwd'
        sh 'ls -al'
        sh 'chmod +x gradlew'
      }
    }
    stage('Test') {
      steps {
        withGradle {
          sh './gradlew clean test'
        }
      }
    }
  }
}