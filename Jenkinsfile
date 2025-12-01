pipeline{
  agent any

  tools{
         maven 'maven'
	     jdk 'java-11'
}

stages{
   stage('git-checkout'){
	steps{
           git branch: 'version-1', url:'https://github.com/vikasmb14/java.git'
             }
   }
   stage('compile'){
        steps{
          sh "mvn compile"
             }
   }
   stage('build'){
        steps{
          sh "mvn package"
            }
      }
  }
}


