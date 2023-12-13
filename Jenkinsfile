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

stage ("slack-bot") {
	step {
		slackSend message: "The build has finished runnig hayaaaa"
	}
}




     }

            }