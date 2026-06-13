pipeline{
	agent any

        tools {
            maven 'maven'
			jdk 'java-11'
         }

	stages{
		stage('git-checkout'){
		 steps{
		 	git branch: 'main', url:'https://github.com/vikasmb14/java.git'
		 }
	   }
	    stage('compile'){
	    	steps{
	    		sh "mvn compile"
	    	}
	    }
        stage('buils'){
        	steps{
        		sh "mvn package"
        	}
        }
	}
}
