pipeline {
  agent any
  stages {
    stage('Unit Test') { 
      steps {
        sh 'mvn clean test'
      }
    }
    stage('Deploy CloudHub') { 
      steps {
        sh 'mvn package deploy -DmuleDeploy'
      }
    }
  }
}