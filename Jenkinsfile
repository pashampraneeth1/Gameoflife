pipeline{
  agent any
  stages{
    stage('checkout'){
      steps{
       git 'https://github.com/pashampraneeth1/Gameoflife.git'
      }
    }
      stage ('Compile'){
         steps{
            sh 'mvn compile' 
         } 
      }
      stage ('Code quality'){
         steps{
            sh 'echo Sonarqube code quality Checkdone' 
         } 
      }
      stage ('Test'){
         steps{
            sh 'mvn test' 
         } 
      }
  }
}

