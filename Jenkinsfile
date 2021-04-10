pipeline{
  agent any
  stages{
      stage ('Compile'){
         agent any
         steps{
            sh 'maven compile' 
         } 
      }
      stage ('Code quality'){
         agent any
         steps{
            sh 'echo Sonarqube code quality Checkdone' 
         } 
      }
      stage ('Test'){
         agent any
         steps{
            sh 'maven test' 
         } 
      }
      stage ('Package'){
         agent any
         steps{
            sh 'maven Package' 
         } 
      }
  }
}

