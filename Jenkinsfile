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
    options { timeout(time: 30, unit: 'MINUTES')}
    stages {

    //    stage('Initialise')
    //         {
    //             steps {
    //                 stepInitialise()
    //             }}
    stage('ContinuousDownload') 
    {
        steps {
         git 'https://github.com/selenium-saikrishna/maven.git'
        }
    }
    stage('ContinuousBuild') 
  
   {
       steps{
    def mavenHome = tool name: "Maven-3.8.6", type: "maven"
    def mavenCMD = "${mavenHome}/bin/mvn"
    sh "${mavenCMD} clean package"
}
        }
    
}
}




