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

stage ("Slack") {

steps{

SlackSend message: 'This is nothing but a test of the jenkins slack integration!'

}

}



	}
}
