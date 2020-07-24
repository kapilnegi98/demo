pipeline {

    agent any
    tools {
        maven 'apache-maven-3.6.3' 
    }
    stages {

	 stage ('Checkout') {
            steps {
                git branch: 'master', url: "D:/java-maven-app/java-maven-app-master/"
            }
        }
           stage('Build stage') {
            steps {
                bat "mvn compile" 
        }
    }

         stage('testing stage') {
             steps {
                bat "mvn test"
        }
    }
}
 }
  
