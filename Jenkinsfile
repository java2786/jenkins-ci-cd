pipeline {

    agent any
    tools {
    	maven 'maven3' 
    }
    
    stages {
    	stage('download') {
    		steps {
    			git 'https://github.com/java2786/jenkins-ci-cd'
    		}
    	}

    	stage('clean') {
    		steps {
    			bat "mvn clean"
    		}
    	}
    	stage('test') {
    		steps {
    			bat "mvn test"
    		}
    	}
    }

}