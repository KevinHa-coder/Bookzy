 pipeline {
	agent any
	stages {
    	stage('Build') {
        	steps {
        	sh "mvn compile"  	 
        	}
    	}
    	stage("Unit test") {          	 
        	steps {  	 
            	sh "mvn test"          	 
       	    }
        }
    	stage("Deploy") {          	 
        	steps {  	 
            	sh "mvn package"  	 
       	    }
        }
    }
}
