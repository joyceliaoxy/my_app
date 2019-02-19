pipeline {
  agent any
  stages {
    stage('---clean---') {
      withEnv(["PATH+mvn=/usr/local/bin"]) {
        sh "mvn clean"
      }
    }
    stage('---test---') {
      withEnv(["PATH+mvn=/usr/local/bin"]) {
        sh "mvn test"
      }
    }
    stage('---package---') {
      withEnv(["PATH+mvn=/usr/local/bin"]) {
        sh "mvn package"
      }
    }
  }
}
