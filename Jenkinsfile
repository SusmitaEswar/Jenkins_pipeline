pipeline {
  agent any
  environment {
		TEST = "pipeline_env"
	}
	stages {
		stage('build and test') {
			parallel {
				stage ('Build') {
					steps {
				        sh 'echo STAGE 1: "hi this is $TEST"'
				}
			}				

				stage ('Test') {
				environment {
					TEST = "test_environment"
				}
					steps {
						sh 'echo STAGE 2: "Test, this is $TEST"'
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