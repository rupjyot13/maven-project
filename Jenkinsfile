pipeline
{

 agent any
 {


stage "scm checkout" {
git 'https://github.com/rakshit2607/maven-project.git'
}

stage "Code Test" {
withMaven(maven: 'LocalMaven') {
    sh  'mvn test'
	}

}
}
}
