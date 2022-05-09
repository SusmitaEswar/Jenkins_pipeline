pipeline {
  agent any
	stages {
		stage('build and test') {
			parallel {
				stage ('Build') {
					steps {
				        sh 'echo STAGE 1: "hi"'
				}
			}				

				stage ('Test') {
					steps {
						sh 'echo STAGE 2: "Test"'
				}
			}
		}
	}	
	stage('depoly') {
	
        steps {
				sh 'echo STAGE 3: "Deploy"'
			}
		}
	}
}