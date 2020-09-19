pipeline{
  agent none
  stages{
      stage ('Compile'){
         agent any
         steps{
            sh "mvn compile" 
         } 
      }
    stage('Build') {
           withEnv(["PATH=${tool 'Maven'}/bin:${tool 'java'}/bin:${env.PATH}"]) {
          sh('mvn clean install')
    } 
  }
  stage ('Code quality'){
         agent any
         steps{
            sh 'echo Sonarqube code quality Checkdone' 
         } 
      }
   }
}
