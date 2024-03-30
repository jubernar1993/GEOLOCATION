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


 stage ("Slack_Notification") {
 
 steps{

	 slackSend color: 'good' , message: "This is a Jenkins Build Test. Please ignore!!!"
 }
 
 
 }



		


	}
}
