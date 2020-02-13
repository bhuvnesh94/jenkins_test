pipeline {
  agent {
    label 'jenkins-slave'
  }
  stages {
     
    stage('init') {
      steps {sh  "sudo docker build . -t test:v1"}
    }
    stage('container launch') {
      steps {sh  "sudo docker  run -d --name nginx1 -p 8082:80  test:v1"}
    }
  }
}