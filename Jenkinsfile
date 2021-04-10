pipeline{
  agent any
  stages{
      stage ('Compile'){
         agent any
         steps{
            sh 'mvn compile' 
         } 
      }
      stage ('Code quality'){
         agent any
         steps{
            sh 'echo Sonarqube code quality Checkdone' 
         } 
      }
      stage ('Test'){
         steps{
            sh 'mvn test' 
         } 
      }
      stage ('Package')
         steps{
            sh 'mvn Package' 
         } 
      }
  }
}

