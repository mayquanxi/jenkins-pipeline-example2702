pipeline {
	agent any
	environment {
		MY_NAME='NGUYEN KHAC MANH'
	}

	stages {
		stage('Buiding') {
			environment {
				LAST_NAME='MANH'
			}
			steps {
				echo '${MY_NAME}'
				echo ' hello ${LAST_NAME}'
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