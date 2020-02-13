pipeline {
  agent {
    label 'jenkins-slave'
  }
  stages {
     
    stage('init') {
      steps {sh  "docker build . -t test:v1"}
    }
    stage('container launch') {
      steps {sh  "docker  run -d --name nginx1 -p 8082:80  test:v1"}
    }
  }
}