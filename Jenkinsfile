pipeline
{
    agent any
    stages
    {
    stage('scm'){
        steps
        {
        git 'https://github.com/snteja/Gameoflife.git'
        }
    }
    stage('build'){
        steps
        {
        sh 'mvn package'
        }
    }

	}
}
