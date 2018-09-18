pipeline {
	agent {
		label ""
	}

	stages {
		stage("Checkout") {
			echo "Checkout SCM"
			checkout scm
		}

		stage("Build") {
			echo "Build Project"
			sh "go build"
		}

		stage("Test") {
			echo "Test Project"
		}

		stage("Deploy to Artifactory") {
			echo "Deploy to Artifactory"
		}
	}
}
