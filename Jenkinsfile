pipeline {
	agent any
stages {

	stage ("clean"){

       when {
		branch 'main'
	   }


		steps{
			sh "echo "this is the main branch" 
		}
	}

stage ("test"){
	steps {

when {
	branch 'dev'
}

		sh "echo "this is the dev"
	}
}


stage ("package"){

	steps {

when {
	branch 'feature-one'
}

		sh "echo "this is the feature-one" "
	}

}
 } 
  }
