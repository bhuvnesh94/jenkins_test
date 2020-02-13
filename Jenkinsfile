pipeline {
  agent {
    label 'jenkins-slave'
  }
  stages {
     
    stage('init') {
      steps {sh  "docker build . -t test:v1"}
    }
    stage('compose up') {
      steps {sh  "docker-compose up -d"}
    }
  }
}