//Declarative//
pipeline{
   agent any
   stages{
      stage('build'){
	steps{
	   echo "Lets build game-of-life"
	   sh 'mvn clean'
	}
      }
     stage('Test'){
      steps{
	 archive "**/target/*.jar"
	 junit 'target/surefire-reports/*.xml'
      }
     }
  }
}
