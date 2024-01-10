pipeline {
	agent any
tools { 
      maven '/opt/maven' 
      jdk '/usr/lib/jvm/java-17-amazon-corretto.x86_64' 
    }
stages {

	stage ("clean"){
		steps{
			sh "mvn clean"
		}
	}

stage ("test"){
	steps {
		sh "mvn test"
	}
}


stage ("package"){

	steps {
		sh "mvn package"
	}

}
 } 
  }
