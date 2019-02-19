pipeline {
  agent any
  stages {
    stage('---clean---') {
      steps {
        withEnv(["PATH+mvn=/usr/local/bin"]) {
          sh "mvn clean"
        }
      }
    }
    stage('---test---') {
      steps {
        withEnv(["PATH+mvn=/usr/local/bin"]) {
          sh "mvn test"
        }
      }
    }
    stage('---package---') {
      steps {
        withEnv(["PATH+mvn=/usr/local/bin"]) {
          sh "mvn package"
        }
      }
    }
  }
}
