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


post {
        success {
            slackSend(channel: '#general', message: "Build succeeded! :white_check_mark:")
        }
        
        failure {
            slackSend(channel: '#general', message: "Build failed! :x:")
        }
    }
}





}


stage ("packageing Stage") {
	steps {
		sh "mvn package"
}

   }

stage ("slack-bot") {
	steps {
		slackSend message: "The build has finished runnig hayaaaa"
	}
}




     }

            