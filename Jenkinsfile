pipeline {
  agent any
	stages {
		stage ('Build') {
			steps {
				    sh '''
							echo STAGE 1: "hi"
							sleep 5
					   '''
					
			}
		}				

		stage ('Test') {
			steps {
					sh '''
							echo STAGE 2: "Test"
							sleep 5
					   '''
			}
		}
			
		stage('deploy') {
			steps {
					sh '''
							echo STAGE 3: "Deploy"
							sleep 5
					   '''
			}
		}
	}
}
