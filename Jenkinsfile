///node('built-in') 
//{
//    stage('Continuous Download') 
//	{
//    git 'https://github.com/sunildevops77/maven.git'
//	}
//    stage('Continuous Build') 
//	{
//    sh 'mvn package'
//	}

//}

pipeline
{
    agent any

    stage('ContinuousDownload') 
    {
         git 'https://github.com/selenium-saikrishna/maven.git'
    }
    stage('ContinuousBuild') 
    {
         sh 'mvn clean package'
    }
}
