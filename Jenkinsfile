pipeline {
  agent any
  stages {
    stage('Unit Test') { 
      steps {
        mvn clean test
      }
    }
    stage('Deploy CloudHub') { 
      steps {
        mvn package deploy -DmuleDeploy
      }
    }
  }
}
