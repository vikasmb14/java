pipeline{
	agent any

        tool {
            maven 'maven'
         }

	stages{
		stage('git-checkout'){
		 steps{
		 	git branch: 'main', url:'https://github.com/vikasmb14/java.git'
		 }
	   }
	    stage('compile'){
	    	steps{
	    		sh "mvm compile"
	    	}
	    }
        stage('buils'){
        	steps{
        		sh "mvn package"
        	}
        }
	}
}
