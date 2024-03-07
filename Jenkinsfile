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




        stage('slack') {
            steps {
            slackSend color: 'good' , message:    'XXXXSimulation a danger or something went right!!!XXXX'
            }
        }



	}
}
