pipeline {
	agent any

	stages {
		stage('Buiding') {
			steps {
				echo 'Buiding'
			}
		}
		stage('Example') {
            steps {
                echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            }
        }
		stage('Deploying') {
			steps {
				echo 'Deploying'
			}
		}
	}
}