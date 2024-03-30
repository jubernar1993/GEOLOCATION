pipeline {
	agent any

	stages {
 
     stage ("Clean") {
		steps {
			sh "mvn clean"
		}
	 }


	 stage ("test") {
		steps{
			sh "mvn test"
		}
	 }

	 stage ("package"){
		steps{
			sh "mvn package"
		}
	 }




	}
}
