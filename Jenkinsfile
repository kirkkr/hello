pipeline {
	agent {
		label ""
	}

	stages {
		stage("Checkout") {
		  steps {
			  echo "Checkout SCM"
			  checkout scm
			}
		}

		stage("Build") {
		  steps {
			  echo "Build Project"
			  sh "go build"
			}
		}

		stage("Test") {
		  steps {
			  echo "Test Project"
			}
		}

		stage("Deploy to Artifactory") {
		  steps {
			  echo "Deploy to Artifactory"
			}
		}
	}
}
