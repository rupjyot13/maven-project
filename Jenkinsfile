pipeline
{

 agent any
 stages
 {


stage ("scm checkout") {
git 'https://github.com/rakshit2607/maven-project.git'
}
}
}

stage ("Code Test") {

steps {
withMaven(maven: 'LocalMaven') 
    {
    sh  'mvn test'
	}
	}
}
}
}
