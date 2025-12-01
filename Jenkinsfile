pipeline{
agent any
tools{
  maven 'maven'
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
   stage('packaging'){
        steps{
          sh"mvn package"
            }
  }
}
}


