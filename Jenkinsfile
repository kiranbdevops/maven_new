pipeline
{
    agent any
    stages
    {
        stage('ContDownload')
        {
            steps
            {
                git 'https://github.com/sunildevops77/maven.git'
            }
        }
		stage('ContBuild')
        {
            steps
            {
                sh 'mvn package'
            }
        }
    }
}

