pipeline {
	agent any

	stages {
 
     stage ("Maven Package") {
		steps {
			sh "mvn clean"
			sh "mvn install"
			sh "mvn package"
		}
	 }


	 stage ("Maven test stage") {
		steps{
			sh "mvn test"
		}
	 }

	 stage ("Deploy"){
		steps{
			echo "Deploying"
		}
	 }


stage ("Slack_notification") {

steps {
	slackSend color: "good" , message: "This is a test to check the capabilities of the slack Notifications!"
}

}


		


	}
}
