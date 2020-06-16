pipeline {
  agent any
  stages {
    stage('Unit Test') { 
		echo ' ENtering Unit Test Stage'
      steps {
		echo 'In Unit Test'
        bash 'mvn clean test'
		echo 'Completed Unit Test Stage'
      }
    }
    stage('Deploy CloudHub') { 
		echo 'Entering Deploy CH Stage'
      steps {
		echo 'firing mv package deploy command'
        bash 'mvn package deploy -DmuleDeploy'
		echo 'mvn packgae deploy completed'
      }
    }
  }
}
