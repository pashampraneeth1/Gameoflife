pipeline{
  agent none
  stages{
      stage ('Compile'){
         agent any
         steps{
            sh "mvn compile" 
         } 
      }
      stage ('Code quality'){
         agent any
         steps{
            sh "echo Sonarqube code quality Checkdone" 
         } 
      }
      stage ('Test'){
         agent any
         steps{
            sh "mvn test" 
         } 
      }
      stage ('Package'){
         agent any
         steps{
            sh "mvn Package" 
         } 
      }
  }

}
