pipeline {
  agent any
  stages {
    stage('Unit Test') { 
	steps {
		echo "*******In Unit Test*************"
        bat "mvn clean test"
		echo "*********Completed Unit Test Stage**********"
      }
    }
    stage('Deploy CloudHub') { 
	steps {
		echo "************firing mv package deploy command*******"
        bat "mvn package deploy -DmuleDeploy"
		echo "*********mvn packgae deploy completed***********"
      }
    }
  }
}
