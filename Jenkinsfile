node('built-in')
{ 
	
	stages{
		stage{
			git branch: 'feature/kiran', url: 'https://github.com/kiranbdevops/maven_new.git'
		}
	  }
	stage(build'){
	      stage{
	      sh 'mvn package'}
	      }
	
}
