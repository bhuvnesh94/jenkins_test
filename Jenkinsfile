pipeline {
  agent any
  stages {
    stage('init') {
      steps {sh  "docker build . -t nginx:v1"}
    }
    stage('compose up') {
      steps {sh  "docker-compose up -d"}
    }
  }
}
