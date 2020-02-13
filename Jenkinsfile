pipeline {
  agent {
    label 'jenkins-slave'
  }
  stages {
     
    stage('init') {
      steps {sh  "sudo docker build . -t test:v1"}
    }
    stage('compose up') {
      steps {sh  "sudo docker-compose up -d"}
    }
  }
}