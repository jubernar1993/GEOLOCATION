pipeline {

agent any

stages {

stage ("cleaning Stage") {
	steps {
		sh "mvn clean"
	}
}
 stage('Build') {
            steps {
                sh "mvn build"
            }
        }
    }
    
    post {
        success {
            slackSend(channel: '#general', message: "yup yup yup we did it! :white_check_mark:")
        }
        
        failure {
            slackSend(channel: '#general', message: "damn it bro! it failed :x:")
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
	steps {
		slackSend message: "The build has finished runnig hayaaaa"
	}
}




     }

            }