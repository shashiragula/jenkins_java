pipeline {
  agent none

  environment {
    MAJOR_VERSION = 1
  }

  stages {
    stage('Say Hello') {
      agent any

      steps {
        echo 'Awesome Student!'
      }
    }
    stage("Test on Debian") {
      agent {
        docker 'openjdk:8u121-jre'
      }
      steps {
       sh "java -version"
      }
    }
  }
}
