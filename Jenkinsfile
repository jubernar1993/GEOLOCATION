pipeline {

agent any

stages {

stage ("cleaning Stage") {
	steps {
		sh "mvn Clean"
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