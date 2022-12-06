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
                sh 'mvn clean'
            }
        }
		stage('ContBuild2')
        {
            steps
            {
                sh 'mvn compile'
            }
        }
		stage('ContBuild3')
        {
            steps
            {
                sh 'mvn package'
            }
        }
    }
}
