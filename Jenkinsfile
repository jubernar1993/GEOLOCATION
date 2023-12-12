pipeline {

agent any

stages {

stage ("cleaning Stage") {
	steps {
		sh "mvn clean"
	}
}


stage ("testing Stage") {

 steps {
	sh "mvn test"
 }

}


stage ("packageing Stage") {
	steps {
		sh "mvn package"
}

   }

     }

            }