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
	        sh "cp /home/labsuser/jenkins/workspace/Bookzy/target/*.war ~/Downloads/apache-tomcat-10.0.6/webapps/"
       	    }
        }
    }
}
