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
            slackSend message: "Build succeeded! :white_check_mark:"
        }
        
        failure {
            slackSend message: "Build failed! :x:"
        }
    }
}





}


stage ("packageing Stage") {
	steps {
		sh "mvn package"
}

   }




     }