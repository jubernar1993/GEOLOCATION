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

stage('slack-bot') {
  
  post {
    aborted {
      slackSend message: "This Build has failed"
    }
    failure {
      slackSend message: "This Build has failed"
    }
    unsuccessful {
      slackSend message: "This Build has failed"
    }
  }
}





     }

            }