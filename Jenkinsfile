pipeline
{

 agent any
 stages
 {


stage ("scm checkout") {
git 'https://github.com/rupjyot13/maven-project'
}

 }
 
 
{

stage ("Code Test") {

steps {
withMaven(maven : 'LocalMaven') 
    {
    sh  'mvn test'
	}
	  }
	                }
}


{					
stage ("Package") {

steps {
withMaven(maven : 'LocalMaven')
   {
   sh 'mvn package'
   }					
					
	   }			
                 }
}
}
